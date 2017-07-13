<span data-ttu-id="59b6a-p119">Envie um código de status `202 - Accepted` na sua resposta para o Microsoft Graph. Se o Microsoft Graph não receber um código de classe 2xx, ele tentará reenviar a notificação várias vezes.</span><span class="sxs-lookup"><span data-stu-id="59b6a-p119">Send a `202 - Accepted` status code in your response to Microsoft Graph. If Microsoft Graph doesn't receive a 2xx class code, it will retry resending the notification a number of times.</span></span>
3. Envie um código de status `202 - Accepted` na sua resposta para o Microsoft Graph. Se o Microsoft Graph não receber um código de classe 2xx, ele tentará reenviar a notificação várias vezes.
  > <span data-ttu-id="59b6a-198">Você deve enviar um código de status `202 - Accepted` mesmo que a propriedade clientState não corresponda àquela enviada com a solicitação de assinatura.</span><span class="sxs-lookup"><span data-stu-id="59b6a-198">You should send a `202 - Accepted` status code even if the clientState property doesn't match the one submitted with the subscription request.</span></span>

<span data-ttu-id="59b6a-199">Repita o procedimento para outras notificações na solicitação.</span><span class="sxs-lookup"><span data-stu-id="59b6a-199">Repeat for other notifications in the request.</span></span>

# <span data-ttu-id="59b6a-200">Recursos adicionais</span><span class="sxs-lookup"><span data-stu-id="59b6a-200">Additional resources</span></span>
<a id="additional-resources" class="xliff"></a>

* [<span data-ttu-id="59b6a-201">Tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="59b6a-201">Subscription resource type</span></span>](subscription.md)
* [<span data-ttu-id="59b6a-202">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="59b6a-202">Get subscription</span></span>](../api/subscription_get.md)
* [<span data-ttu-id="59b6a-203">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="59b6a-203">Create subscription</span></span>](../api/subscription_post_subscriptions.md)
* [<span data-ttu-id="59b6a-204">Exemplo de webhooks do Microsoft Graph para Node.js</span><span class="sxs-lookup"><span data-stu-id="59b6a-204">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [<span data-ttu-id="59b6a-205">Exemplo de webhooks do Microsoft Graph para ASP,NET</span><span class="sxs-lookup"><span data-stu-id="59b6a-205">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
