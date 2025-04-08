---
description: >-
  Add the HQ chatbot to your helpdesk tool and handle support questions more
  easily
icon: sliders-up
---

# Setting up the HQ chatbot

The _Intelligent Chatbot_ feature is an AI-driven tool that automatically handles customer inquiries on your e-commerce platform.&#x20;

It can respond to frequently asked questions, provide order statuses, troubleshoot common issues, and escalate more complex problems to human agents when necessary.

The chatbot is customizable and integrates seamlessly with your existing ticketing system, ensuring that every interaction is tracked and monitored.

You can also [integrate the chatbot into your website](setting-up-the-hq-chatbot.md#integrate-the-chatbot-into-your-website) — read on to find out how.

***

### **How to use the chatbot**

Below is a step-by-step guide to setting up and using the Intelligent Chatbot feature on your SaaS platform.

{% stepper %}
{% step %}
### Create a new chatbot

[Log in to your account](https://www.headquarters.com/login) and navigate to the main dashboard. Under the "Support" tab, click on **Chatbot Settings**, then select **New Chatbot** to create a customized bot for your e-commerce store. You’ll be prompted to select a template or start from scratch.
{% endstep %}

{% step %}
### Configure responses

The system offers multiple templates for common customer questions, such as order status inquiries, shipping details, and return policies. Select the relevant templates based on your business needs.
{% endstep %}

{% step %}
### Set up custom responses

You can also define custom responses for any other type of inquiry. For example, if your customers frequently ask about product materials or size guides, you can input responses in the "Custom Responses" section.
{% endstep %}

{% step %}
### Test the chatbot

Once you've configured your chatbot, switch it to "Test Mode" to see how it performs in a simulated environment. This ensures the bot understands customer inputs correctly and responds appropriately.

If any responses are incorrect or unclear, return to the "Response Settings" page to fine-tune the chatbot's language and logic.
{% endstep %}
{% endstepper %}

***

### **Integrate the chatbot into your website**

{% stepper %}
{% step %}
### Create & copy the chatbot code

Once your chatbot is configured and tested, navigate to the **Integration** section of the Chatbot Settings page. Here, you'll find a JavaScript snippet that allows you to embed the chatbot on your e-commerce website. Click the **Copy** button to copy the integration code.
{% endstep %}

{% step %}
### Add the code to your website

Open the HTML file or the template file for the web page(s) where you want the chatbot to appear. Paste the copied JavaScript code just before the closing `</body>` tag of your website's HTML file.

```html
<!-- Insert Chatbot Script -->
<script type="text/javascript">
    (function(d, w, c) {
        w.ChatbotSettings = {
            token: 'YOUR_CHATBOT_TOKEN',  // Replace with your token
            position: 'bottom-right',   // Customize position
            color: '#009688',           // Customize bot color
            language: 'en'              // Customize language
        };
        var s = d.createElement('script');
        s.src = 'https://cdn.yourchatbot.com/widget.js';
        s.async = true;
        d.head.appendChild(s);
    })(document, window);
</script>
```

After pasting the code, save your file and deploy the changes to your web server. The chatbot should now appear on your website for users to interact with.
{% endstep %}

{% step %}
### Optimize your settings

Once the chatbot is live, head to the "Analytics" tab on your SaaS platform dashboard. Here you can monitor key performance metrics like:

* Number of queries handled
* Common customer questions
* Escalation rate to human agents
{% endstep %}

{% step %}
### Monitor performance

Based on the chatbot's performance, you can return to the Chatbot Settings to update responses, add new templates, or adjust bot behavior for improved customer satisfaction.
{% endstep %}
{% endstepper %}

***

### **Next Steps**

* **Advanced Customization:** Learn how to implement advanced features like natural language processing (NLP) and multi-lingual support in your chatbot.
* **Connect to CRM:** Integrate the chatbot with your CRM system to sync customer interactions and gather deeper insights into user behavior.

For further details or troubleshooting, refer to our [Support Documentation](https://app.gitbook.com/o/d8f63b60-89ae-11e7-8574-5927d48c4877/s/zq8ynchcecIscc4uulgN/) or [contact our helpdesk](mailto:support@headquarters.com).
