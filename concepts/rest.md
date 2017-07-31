<span data-ttu-id="32c19-p119">Agora que você viu como fazer chamadas ao Microsoft Graph, pode usar a referência de API para construir outros tipos de chamada que seu aplicativo tenha que fazer. No entanto, tenha em mente que seu aplicativo precisa ter as permissões apropriadas configuradas no registro de aplicativo para as chamadas feitas.</span><span class="sxs-lookup"><span data-stu-id="32c19-p119">Now that you've seen how to make calls to Microsoft Graph, you can use the API reference to construct any other kinds of calls your app needs to make. However, bear in mind that your app needs to have the appropriate permissions configured on the app registration for the calls it makes.</span></span>

```
GET https://graph.microsoft.com/v1.0/me/messages?$select=subject,from,receivedDateTime&$top=25&$orderby=receivedDateTime%20DESC
Accept: application/json
Authorization: Bearer eyJ0eXAi...b66LoPVA
```

Agora que você viu como fazer chamadas ao Microsoft Graph, pode usar a referência de API para construir outros tipos de chamada que seu aplicativo tenha que fazer. No entanto, tenha em mente que seu aplicativo precisa ter as permissões apropriadas configuradas no registro de aplicativo para as chamadas feitas.

## <a name="next-steps"></a><span data-ttu-id="32c19-189">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="32c19-189">Next steps</span></span>
- <span data-ttu-id="32c19-190">Experimente mais da API REST usando o [Explorador do Graph](https://graph.microsoft.io/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="32c19-190">Try out more of the REST API using the [Graph explorer](https://graph.microsoft.io/graph-explorer).</span></span>

## <a name="see-also"></a><span data-ttu-id="32c19-191">Ver também</span><span class="sxs-lookup"><span data-stu-id="32c19-191">See also</span></span>
- [<span data-ttu-id="32c19-192">Protocolos do Azure AD v2.0</span><span class="sxs-lookup"><span data-stu-id="32c19-192">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="32c19-193">Tokens do Azure AD v2.0</span><span class="sxs-lookup"><span data-stu-id="32c19-193">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
