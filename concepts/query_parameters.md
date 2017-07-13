<span data-ttu-id="b0244-p117">Os critérios de pesquisa são expressos usando a sintaxe de consulta avançada (AQS). Os resultados são classificados pela data e hora em que a mensagem foi enviada.</span><span class="sxs-lookup"><span data-stu-id="b0244-p117">Search criteria are expressed using Advanced Query Syntax (AQS). The results are sorted by the date and time that the message was sent.</span></span>

Os critérios de pesquisa são expressos usando a sintaxe de consulta avançada (AQS). Os resultados são classificados pela data e hora em que a mensagem foi enviada.

<span data-ttu-id="b0244-194">Você pode especificar as seguintes propriedades em uma `message` em um critério `$search`: `attachments`, `bccRecipients`, `body`, `category`, `ccRecipients`, `content`, `from`, `hasAttachments`, `participants`, `receivedDateTime`, `sender`, `subject`,`toRecipients`</span><span class="sxs-lookup"><span data-stu-id="b0244-194">You can specify the following properties on a `message` in a `$search` criterion: `attachments`, `bccRecipients`, `body`, `category`, `ccRecipients`, `content`, `from`, `hasAttachments`, `participants`, `receivedDateTime`, `sender`, `subject`, `toRecipients`</span></span>

<span data-ttu-id="b0244-195">Se você realizar uma pesquisa em mensagens e especificar apenas um valor, a pesquisa será realizada nas propriedades de pesquisa padrão `from`, `subject` e `body`.</span><span class="sxs-lookup"><span data-stu-id="b0244-195">If you do a search on messages and specify only a value, the search is carried out on the default search properties of `from`, `subject` and `body`.</span></span>

<span data-ttu-id="b0244-196">O exemplo a seguir retorna todas as mensagens na Caixa de Entrada do usuário que contenham "pizza" em qualquer uma das três propriedades de pesquisa padrão:</span><span class="sxs-lookup"><span data-stu-id="b0244-196">The following example returns all messages in the signed-in user's Inbox that contains "pizza" in any of the three default search properties:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

<span data-ttu-id="b0244-197">O próximo exemplo procura todas as mensagens na Caixa de Entrada do usuário que foram enviadas de um endereço de email específico:</span><span class="sxs-lookup"><span data-stu-id="b0244-197">The next example searches all messages in the user's Inbox that were sent from a specific email address:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="from:help@contoso.com"
```

[graph-explorer]: https://graph.microsoft.io/en-us/graph-explorer
[odata-filter]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356
