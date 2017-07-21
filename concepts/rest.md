<span data-ttu-id="bab8b-p119">Agora que você viu como fazer chamadas ao Microsoft Graph, pode usar a referência de API para construir outros tipos de chamada que seu aplicativo tenha que fazer. No entanto, tenha em mente que seu aplicativo precisa ter as permissões apropriadas configuradas no registro de aplicativo para as chamadas feitas.</span><span class="sxs-lookup"><span data-stu-id="bab8b-p119">Now that you've seen how to make calls to Microsoft Graph, you can use the API reference to construct any other kinds of calls your app needs to make. However, bear in mind that your app needs to have the appropriate permissions configured on the app registration for the calls it makes.</span></span>

```
GET https://graph.microsoft.com/v1.0/me/messages?$select=subject,from,receivedDateTime&$top=25&$orderby=receivedDateTime%20DESC
Accept: application/json
Authorization: Bearer eyJ0eXAi...b66LoPVA
```

Agora que você viu como fazer chamadas ao Microsoft Graph, pode usar a referência de API para construir outros tipos de chamada que seu aplicativo tenha que fazer. No entanto, tenha em mente que seu aplicativo precisa ter as permissões apropriadas configuradas no registro de aplicativo para as chamadas feitas.

## <a name="next-steps"></a><span data-ttu-id="bab8b-189">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="bab8b-189">Next steps</span></span>
- <span data-ttu-id="bab8b-190">Experimente mais da API REST usando o [Explorador do Graph](https://graph.microsoft.io/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="bab8b-190">Try out more of the REST API using the [Graph explorer](https://graph.microsoft.io/graph-explorer).</span></span>

## <a name="see-also"></a><span data-ttu-id="bab8b-191">Ver também</span><span class="sxs-lookup"><span data-stu-id="bab8b-191">See also</span></span>
- [<span data-ttu-id="bab8b-192">Obter tokens de acesso para chamar o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="bab8b-192">Get access tokens to call Microsoft Graph</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_overview)
- [<span data-ttu-id="bab8b-193">Obter acesso em nome de um usuário</span><span class="sxs-lookup"><span data-stu-id="bab8b-193">Get access on behalf of a user</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_user)
- [<span data-ttu-id="bab8b-194">Obter acesso sem um usuário</span><span class="sxs-lookup"><span data-stu-id="bab8b-194">Get access without a user</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_service)
