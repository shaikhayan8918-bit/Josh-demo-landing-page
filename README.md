# Josh-demo-landing-page
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>From Skinny-Fat to Strong in 90 Days</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            background-color: #f8f9fa;
        }
        
        .container {
            max-width: 900px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        .section {
            padding: 60px 0;
            background: white;
            margin-bottom: 2px;
        }
        
        .hero {
            background: linear-gradient(135deg, #1e3c72 0%, #2a5298 100%);
            color: white;
            text-align: center;
            padding: 80px 0;
        }
        
        .preheader {
            font-size: 16px;
            color: #ffd700;
            font-weight: bold;
            margin-bottom: 20px;
            text-transform: uppercase;
            letter-spacing: 1px;
        }
        
        h1 {
            font-size: 3.2rem;
            font-weight: 900;
            line-height: 1.2;
            margin-bottom: 25px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }
        
        .subheader {
            font-size: 1.4rem;
            margin-bottom: 40px;
            color: #e8f4fd;
            font-weight: 300;
        }
        
        .vsl-container {
            margin: 40px 0;
        }
        
        .vsl-icon {
            display: inline-block;
            position: relative;
            cursor: pointer;
            transition: transform 0.3s ease;
        }
        
        .vsl-icon:hover {
            transform: scale(1.05);
        }
        
        .video-thumbnail {
            width: 400px;
            height: 225px;
            background: linear-gradient(45deg, #ff6b6b, #4ecdc4);
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
            box-shadow: 0 10px 30px rgba(0,0,0,0.3);
        }
        
        .play-button {
            width: 80px;
            height: 80px;
            background: rgba(255,255,255,0.9);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }
        
        .play-button::after {
            content: '';
            width: 0;
            height: 0;
            border-left: 25px solid #333;
            border-top: 15px solid transparent;
            border-bottom: 15px solid transparent;
            margin-left: 5px;
        }
        
        .vsl-text {
            margin-top: 15px;
            font-size: 1.1rem;
            color: #ffd700;
            font-weight: bold;
        }
        
        .cta-button {
            display: inline-block;
            background: #ff4757;
            color: white;
            padding: 20px 40px;
            font-size: 1.3rem;
            font-weight: bold;
            text-decoration: none;
            border-radius: 8px;
            margin-top: 30px;
            transition: all 0.3s ease;
            box-shadow: 0 5px 20px rgba(255,71,87,0.4);
            text-transform: uppercase;
            letter-spacing: 1px;
        }
        
        .cta-button:hover {
            background: #ff3742;
            transform: translateY(-2px);
            box-shadow: 0 8px 25px rgba(255,71,87,0.6);
        }
        
        h2 {
            font-size: 2.5rem;
            margin-bottom: 30px;
            color: #2c3e50;
            font-weight: 800;
        }
        
        .fascination {
            color: #e74c3c;
            font-style: italic;
        }
        
        p {
            font-size: 1.1rem;
            margin-bottom: 20px;
            color: #555;
        }
        
        .emphasis {
            font-weight: bold;
            color: #2c3e50;
        }
        
        .caps {
            text-transform: uppercase;
            font-weight: bold;
            color: #e74c3c;
        }
        
        .bullet-point {
            background: #f8f9fa;
            border-left: 4px solid #3498db;
            padding: 20px;
            margin: 20px 0;
            border-radius: 0 8px 8px 0;
        }
        
        .bullet-feature {
            font-weight: bold;
            color: #2c3e50;
            font-size: 1.1rem;
        }
        
        .value-stack {
            background: #f1f2f6;
            padding: 30px;
            border-radius: 12px;
            margin: 30px 0;
            border: 2px solid #ddd;
        }
        
        .value-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 0;
            border-bottom: 1px solid #ddd;
        }
        
        .value-item:last-child {
            border-bottom: none;
            font-weight: bold;
            font-size: 1.2rem;
            color: #e74c3c;
        }
        
        .faq-item {
            background: white;
            border: 1px solid #ddd;
            border-radius: 8px;
            margin: 20px 0;
            overflow: hidden;
        }
        
        .faq-question {
            background: #f8f9fa;
            padding: 20px;
            font-weight: bold;
            color: #2c3e50;
            font-size: 1.1rem;
        }
        
        .faq-answer {
            padding: 20px;
            color: #555;
        }
        
        .guarantee-box {
            background: linear-gradient(135deg, #2ecc71, #27ae60);
            color: white;
            padding: 30px;
            border-radius: 12px;
            text-align: center;
            margin: 40px 0;
            box-shadow: 0 10px 30px rgba(46,204,113,0.3);
        }
        
        .testimonial {
            background: #f8f9fa;
            border-left: 4px solid #3498db;
            padding: 25px;
            margin: 30px 0;
            border-radius: 0 8px 8px 0;
            font-style: italic;
            position: relative;
        }
        
        .testimonial::before {
            content: '"';
            font-size: 4rem;
            color: #3498db;
            position: absolute;
            top: -10px;
            left: 15px;
            opacity: 0.3;
        }
        
        @media (max-width: 768px) {
            h1 {
                font-size: 2.2rem;
            }
            
            h2 {
                font-size: 1.8rem;
            }
            
            .video-thumbnail {
                width: 300px;
                height: 169px;
            }
            
            .container {
                padding: 0 15px;
            }
        }
    </style>
</head>
<body>
    <!-- HERO SECTION -->
    <section class="hero">
        <div class="container">
            <div class="preheader">ATTENTION: Busy Skinny-Fat Men Who've Tried Everything</div>
            
            <h1>Gain 5+ Lbs of Muscle & Drop 10+ Lbs of Fat in 90 Days Without 3-Hour Gym Sessions or Bodybuilder Meal Prep</h1>
            
            <div class="subheader">
                Finally escape the skinny-fat trap using the exact fundamentals that work... without guilt, binge cycles, or wasted time on influencer nonsense
            </div>
            
            <div class="vsl-container">
                <a href="https://docs.google.com/document/d/1ZQqaQRRaFOLMeA-g9XNyFqHqLXJ56pwJ-YuQZd2Qh7A/edit?usp=sharing" class="vsl-icon">
                    <div class="video-thumbnail">
                        <div class="play-button"></div>
                    </div>
                    <div class="vsl-text">Click Here To See The: VSL I WROTE FOR YOU</div>
                </a>
            </div>
            
            <a href="#offer" class="cta-button">Begin Transformation Now</a>
        </div>
    </section>

    <!-- PROBLEM IDENTIFICATION -->
    <section class="section">
        <div class="container">
            <h2 class="fascination">The Skinny-Fat Prison That's Stealing Your Confidence</h2>
            
            <p>You stare in the mirror every morning...</p>
            
            <p>And the same frustrating reality stares back.</p>
            
            <p><span class="emphasis">No muscle definition.</span> Soft around the midsection. Arms that look decent in a shirt but disappear when you take it off.</p>
            
            <p>You've tried everything...</p>
            
            <p>You've followed the celebrity workout that promised "Hollywood abs in 30 days." You've downloaded the influencer's "secret bulking protocol." You've even tried that insane 2-hour daily routine from the fitness YouTuber with 2 million subscribers.</p>
            
            <p>Yet here you are... <span class="emphasis">months later</span>... still trapped in the same skinny-fat body.</p>
            
            <p>And it's not just your physique that's suffering...</p>
            
            <p>You've wasted HUNDREDS of hours in the gym following programs that left you injured, exhausted, and no closer to your goal.</p>
            
            <p>You've blown your hard-earned money on supplement stacks that did absolutely nothing except make your wallet lighter.</p>
            
            <p>You've endured the mental torture of strict meal preps only to crack and binge on everything in sight... then hate yourself for it.</p>
            
            <p><span class="caps">But here's what really keeps you up at night...</span></p>
            
            <p>The fear that maybe you're just not built for this.</p>
            
            <p>That maybe those impressive transformations you see online are only possible for genetic freaks or guys using "extra help."</p>
            
            <p>That maybe you'll spend ANOTHER year spinning your wheels... only to look exactly the same 12 months from now.</p>
            
            <p>But what if I told you there's a proven way out?</p>
            
            <p>What if the solution isn't more intensity, more supplements, or more restriction...</p>
            
            <p><span class="emphasis">But actually the complete opposite?</span></p>
        </div>
    </section>

    <!-- ORIGIN STORY -->
    <section class="section" style="background: #f8f9fa;">
        <div class="container">
            <h2 class="fascination">How I Escaped the Same Prison You're In Right Now</h2>
            
            <p>Two years ago, I was you.</p>
            
            <p>Skinny-fat. Frustrated. Confused by the endless contradictory advice flooding my social media feeds.</p>
            
            <p>I'd spent 18 months jumping from program to program... diet to diet... supplement to supplement.</p>
            
            <p><span class="emphasis">The results?</span> A lighter bank account, chronic shoulder pain from ego-driven lifting, and the exact same soft, undefined physique I started with.</p>
            
            <p>I was ready to give up.</p>
            
            <p>Then something clicked...</p>
            
            <p>I was scrolling through yet another "grow your arms by 5 inches" video when I realized something profound:</p>
            
            <p><span class="emphasis">Every successful transformation I'd studied had the exact same foundation.</span></p>
            
            <p>Not the flashy stuff. Not the "secret techniques" or exotic supplements.</p>
            
            <p>The boring fundamentals.</p>
            
            <p>Consistent calorie tracking. Progressive overload with perfect form. Flexible eating that prevented binge cycles.</p>
            
            <p>But here's the kicker...</p>
            
            <p>The fitness industry makes ZERO money when you succeed with simple fundamentals.</p>
            
            <p>They need you confused, constantly searching for the next "breakthrough" program or miracle supplement.</p>
            
            <p>They need you to believe that transformation requires 3-hour daily gym sessions and eating nothing but chicken, rice, and broccoli.</p>
            
            <p>Because the moment you realize the truth...</p>
            
            <p>The moment you see that sustainable transformation comes from mastering the basics...</p>
            
            <p><span class="emphasis">You stop buying their products.</span></p>
            
            <p>So I ignored everything else and focused solely on what actually worked.</p>
            
            <p>The result? In 12 months, I gained 15 pounds of muscle while dropping 20 pounds of fat.</p>
            
            <p>Working out just 3 times per week. Eating foods I actually enjoyed. Never counting macros down to the gram.</p>
            
            <p>And now I'm going to show you exactly how to do the same thing.</p>
        </div>
    </section>

    <!-- SOLUTION REVELATION -->
    <section class="section">
        <div class="container">
            <h2 class="fascination">The 90-Day Fundamentals Protocol That Actually Works</h2>
            
            <p>Forget everything you think you know about building muscle and losing fat.</p>
            
            <p>Here's what actually happens when you stop chasing shiny objects and focus on what matters:</p>
            
            <p><span class="emphasis">Week 1-2:</span> You'll establish a sustainable calorie deficit while eating foods you actually enjoy. No more guilt. No more binge cycles.</p>
            
            <p><span class="emphasis">Week 3-6:</span> Your body starts responding to intelligent training. Three focused workouts per week, emphasizing perfect form over ego lifting.</p>
            
            <p><span class="emphasis">Week 7-12:</span> The magic happens. Muscle definition emerges. Fat melts off. People start asking what you're doing differently.</p>
            
            <p>But here's what makes this different from every other program you've tried...</p>
            
            <p><span class="caps">It's designed specifically for skinny-fat men who've been burned before.</span></p>
            
            <div class="bullet-point">
                <div class="bullet-feature">Injury-Proof Progressive Overload</div>
                <p>Never again will you sacrifice your shoulder health for an ego-driven bench press. You'll build strength through full range of motion, keeping your joints healthy for decades.</p>
            </div>
            
            <div class="bullet-point">
                <div class="bullet-feature">Flexible Eating Framework</div>
                <p>Eat pizza without guilt. Have drinks with friends without derailing your progress. Finally break free from the restrict-binge cycle that's been sabotaging your results.</p>
            </div>
            
            <div class="bullet-point">
                <div class="bullet-feature">3-Workout Weekly Structure</div>
                <p>Spend just 3-6 hours per week in the gym while making faster progress than guys training twice as much. More results, more free time, more balance.</p>
            </div>
            
            <div class="bullet-point">
                <div class="bullet-feature">Meticulous But Simple Tracking</div>
                <p>Know exactly what's working and what isn't. No more guessing, no more spinning your wheels. Every decision is data-driven and purposeful.</p>
            </div>
            
            <p>The best part?</p>
            
            <p><span class="emphasis">This isn't theory.</span> It's the exact system I used to gain 15 pounds of muscle and lose 20 pounds of fat in 12 months.</p>
            
            <p>And now, for the first time ever, I'm revealing every detail in a step-by-step workshop...</p>
        </div>
    </section>

    <!-- PRODUCT INTRODUCTION -->
    <section class="section" style="background: #f8f9fa;">
        <div class="container">
            <h2 class="fascination">Introducing: The 90-Day Skinny-Fat Solution</h2>
            
            <p>This isn't another generic workout program.</p>
            
            <p>This isn't another restrictive diet plan.</p>
            
            <p>This is the complete roadmap to finally escape the skinny-fat trap using the exact fundamentals that actually work.</p>
            
            <p><span class="emphasis">90 minutes of concise, no-BS video content</span> that cuts through the noise and gives you exactly what you need to know.</p>
            
            <p>No filler. No fluff. No regurgitated Instagram advice.</p>
            
            <p>Just the distilled wisdom from natural bodybuilding coaches, backed by real-world results, packaged into a system you can implement immediately.</p>
            
            <p>Here's what you get:</p>
            
            <div class="bullet-point">
                <div class="bullet-feature">The Skinny-Fat Training Foundation</div>
                <p>The 3-day workout structure that builds muscle in all the right places while keeping you injury-free. You'll never waste time on ineffective exercises again.</p>
            </div>
            
            <div class="bullet-point">
                <div class="bullet-feature">Flexible Nutrition Framework</div>
                <p>How to create a sustainable calorie deficit while eating foods you love. No more meal prep slavery or social isolation.</p>
            </div>
            
            <div class="bullet-point">
                <div class="bullet-feature">Progress Tracking System</div>
                <p>The simple metrics that tell you exactly when to adjust your approach. Stop guessing and start knowing.</p>
            </div>
            
            <div class="bullet-point">
                <div class="bullet-feature">Mindset Shifts That Stick</div>
                <p>Break free from the all-or-nothing mentality that's been sabotaging your progress. Build habits that last a lifetime.</p>
            </div>
            
            <p>This is everything I wish I'd known when I was trapped in my own skinny-fat prison.</p>
            
            <p>The shortcuts that would have saved me 18 months of frustration, hundreds of dollars in useless supplements, and countless hours of ineffective training.</p>
            
            <p><span class="emphasis">It's all yours today.</span></p>
        </div>
    </section>

    <!-- OFFER STRUCTURE -->
    <section class="section" id="offer">
        <div class="container">
            <h2 class="fascination">Everything You Need to Finally Win This Battle</h2>
            
            <div class="value-stack">
                <div class="value-item">
                    <span><strong>The 90-Day Roadmap</strong> - Complete step-by-step transformation guide</span>
                    <span>$197 Value</span>
                </div>
                <div class="value-item">
                    <span><strong>Skinny-Fat Training System</strong> - 3-day workout structure with video demonstrations</span>
                    <span>$147 Value</span>
                </div>
                <div class="value-item">
                    <span><strong>Flexible Nutrition Framework</strong> - Sustainable eating approach that prevents binges</span>
                    <span>$97 Value</span>
                </div>
                <div class="value-item">
                    <span><strong>Progress Tracking Templates</strong> - Know exactly what's working</span>
                    <span>$47 Value</span>
                </div>
                <div class="value-item">
                    <span><strong>My Personal Transformation Video</strong> - Proof this system works</span>
                    <span>$27 Value</span>
                </div>
                <div class="value-item">
                    <span><strong>Total Value:</strong></span>
                    <span>£49.99</span>
                </div>
            </div>
            
            <div class="guarantee-box">
                <h3 style="margin-bottom: 15px;">30-Day Money-Back Guarantee</h3>
                <p>If you don't see noticeable results in the first 30 days, or if you simply prefer the Hollywood approach over proven fundamentals, just email me and I'll refund every penny. No questions asked.</p>
            </div>
            
            <div style="text-align: center; margin: 40px 0;">
                <p style="font-size: 1.3rem; margin-bottom: 20px;"><span class="caps">Limited Time:</span> First 100 men get access for just...</p>
                <p style="font-size: 2.5rem; font-weight: bold; color: #e74c3c; margin-bottom: 30px;">Price Available at Checkout</p>
                <a href="#" class="cta-button">Begin Transformation Now</a>
                <p style="margin-top: 15px; font-size: 0.9rem; color: #666;">Secure checkout - Your information is protected</p>
            </div>
        </div>
    </section>

    <!-- FAQ SECTION -->
    <section class="section" style="background: #f8f9fa;">
        <div class="container">
            <h2 class="fascination">Common Questions From Men Ready to Change</h2>
            
            <div class="faq-item">
                <div class="faq-question">What if I don't have time for 3 workouts per week?</div>
                <div class="faq-answer">
                    <p>If you can't commit to 3-6 hours per week for your health and confidence, this program isn't for you. But if you're currently wasting 10+ hours per week following ineffective routines, you'll actually save time while getting better results.</p>
                </div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">I've tried everything. How is this different?</div>
                <div class="faq-answer">
                    <p>Everything you've tried has been designed to keep you confused and coming back for more. This program gives you the fundamentals once and for all, so you never need another fitness product again. That's exactly why most companies won't teach this stuff.</p>
                </div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">Do I need a full gym membership?</div>
                <div class="faq-answer">
                    <p>Yes. This program requires access to barbells, dumbbells, and basic gym equipment. If you're not willing to invest in a proper gym membership, you're not serious enough about transformation for this to work.</p>
                </div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">What if I prefer the Hollywood celebrity approach?</div>
                <div class="faq-answer">
                    <p>Then get your money back. I'm not here to convince you that fundamentals work better than flashy gimmicks. The 30-day guarantee exists specifically for men who prefer style over substance.</p>
                </div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">How quickly will I see results?</div>
                <div class="faq-answer">
                    <p>Most men notice changes in energy and strength within the first 2 weeks. Visual changes typically appear around week 4-6. By day 90, you'll have the foundation for a complete physique transformation. No magic, just consistent fundamentals.</p>
                </div>
            </div>
            
            <div style="text-align: center; margin-top: 50px;">
                <p style="font-size: 1.2rem; margin-bottom: 30px;">Ready to finally escape the skinny-fat trap?</p>
                <a href="#" class="cta-button">Begin Your Transformation</a>
            </div>
        </div>
    </section>

    <!-- FINAL CTA -->
    <section class="hero">
        <div class="container" style="text-align: center;">
            <h2 style="color: white; margin-bottom: 30px;">Your Transformation Starts Today</h2>
            <p style="font-size: 1.2rem; margin-bottom: 30px; color: #e8f4fd;">Stop wasting time on programs that don't work. Join the men who chose fundamentals over flash and got the results that matter.</p>
            <a href="#" class="cta-button">Begin Transformation Now</a>
        </div>
    </section>
</body>
</html>
