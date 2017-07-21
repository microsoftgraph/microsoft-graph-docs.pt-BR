<span data-ttu-id="75847-p119">Para criar o email, o código obtém o nome de usuário do token de sessão e o endereço de email do destinatário dos parâmetros passados do formulário. O código, em seguida, lê o corpo do email de um modelo incluído no projeto, interpola o endereço de email e o nome de usuário e anexa o texto do email como o corpo da solicitação HTTP.</span><span class="sxs-lookup"><span data-stu-id="75847-p119">To create the email, the code pulls the user name from the session token and the recipient email address from the parameters passed from the form. The code then reads the email body from a template included in the project, interpolates the user name and email address, and attaches the email text as the HTTP request body.</span></span>

Para criar o email, o código obtém o nome de usuário do token de sessão e o endereço de email do destinatário dos parâmetros passados do formulário. O código, em seguida, lê o corpo do email de um modelo incluído no projeto, interpola o endereço de email e o nome de usuário e anexa o texto do email como o corpo da solicitação HTTP.

<span data-ttu-id="75847-194">Para enviar o email, o código constrói a solicitação HTTP, anexa o token de acesso como um cabeçalho de autorização e, em seguida, envia a solicitação para o ponto de extremidade de enviar email.</span><span class="sxs-lookup"><span data-stu-id="75847-194">To send the email, the code constructs the HTTP request, attaches the access token as an authorization header, and then posts the request to the send email endpoint.</span></span>

<span data-ttu-id="75847-195">Por fim, o código usa o código de resposta de HTTP retornado para notificar o usuário se o email foi concluído com êxito ou não.</span><span class="sxs-lookup"><span data-stu-id="75847-195">Finally, the code uses the HTTP response code returned to notify the user whether or not the email was successful.</span></span>

## <a name="run-the-app"></a><span data-ttu-id="75847-196">Executar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="75847-196">Run the app</span></span>

1. <span data-ttu-id="75847-197">Instale o aplicativo Rails e as dependências com o seguinte comando.</span><span class="sxs-lookup"><span data-stu-id="75847-197">Install the Rails application and dependencies with the following command.</span></span>

    ```
    bundle install
    ```
2. <span data-ttu-id="75847-198">Para iniciar o aplicativo Rails, digite o seguinte comando.</span><span class="sxs-lookup"><span data-stu-id="75847-198">To start the Rails application, type the following command.</span></span>

    ```
    rackup -p 3000
    ```
3. <span data-ttu-id="75847-199">Acesse `http://localhost:3000` no navegador da Web.</span><span class="sxs-lookup"><span data-stu-id="75847-199">Go to `http://localhost:3000` in your web browser.</span></span>

## <a name="see-also"></a><span data-ttu-id="75847-200">Ver também</span><span class="sxs-lookup"><span data-stu-id="75847-200">See also</span></span>
- <span data-ttu-id="75847-201">Experimente a API REST usando o [Explorador do Graph](https://graph.microsoft.io/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="75847-201">Try out the REST API using the [Graph explorer](https://graph.microsoft.io/graph-explorer).</span></span>
- <span data-ttu-id="75847-202">Explorar nossos outros [exemplos do Microsoft Graph](https://github.com/microsoftgraph) no GitHub.</span><span class="sxs-lookup"><span data-stu-id="75847-202">Explore our other [Microsoft Graph samples](https://github.com/microsoftgraph) on GitHub.</span></span>
- [<span data-ttu-id="75847-203">Obter tokens de acesso para chamar o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="75847-203">Get access tokens to call Microsoft Graph</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_overview)
- [<span data-ttu-id="75847-204">Obter acesso em nome de um usuário</span><span class="sxs-lookup"><span data-stu-id="75847-204">Get access on behalf of a user</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_user)
- [<span data-ttu-id="75847-205">Obter acesso sem um usuário</span><span class="sxs-lookup"><span data-stu-id="75847-205">Get access without a user</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_service)


