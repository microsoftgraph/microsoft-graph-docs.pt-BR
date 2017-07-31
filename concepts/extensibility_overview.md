<span data-ttu-id="48594-p116">As mesmas [permissões](./permissions_reference.md) necessárias para ler ou gravar um recurso específico também são necessárias para ler ou gravar quaisquer dados de extensões nesse recurso.  Por exemplo, para que um aplicativo seja capaz de atualizar o perfil de um usuário conectado com dados de aplicativo personalizados, o aplicativo deve receber a permissão *User.ReadWrite.All*.</span><span class="sxs-lookup"><span data-stu-id="48594-p116">The same [permissions](./permissions_reference.md) that are required to read from or write to a specific resource are also required to read from or write to any extensions data on that resource.  For example, for an app to be able to update the signed-in user's profile with custom app data, the app must have been granted the *User.ReadWrite.All* permission.</span></span>

As mesmas [permissões](./permissions_reference.md) necessárias para ler ou gravar um recurso específico também são necessárias para ler ou gravar quaisquer dados de extensões nesse recurso.  Por exemplo, para que um aplicativo seja capaz de atualizar o perfil de um usuário conectado com dados de aplicativo personalizados, o aplicativo deve receber a permissão *User.ReadWrite.All*.

<span data-ttu-id="48594-229">Além disso, para criar e gerenciar definições de extensão do esquema, um aplicativo deve receber a permissão *Directory.AccessAsUser.All*.</span><span class="sxs-lookup"><span data-stu-id="48594-229">Additionally, to create and manage schema extension definitions, an application must be granted the *Directory.AccessAsUser.All* permission.</span></span>

## <a name="data-limits"></a><span data-ttu-id="48594-230">Limites de dados</span><span class="sxs-lookup"><span data-stu-id="48594-230">Data limits</span></span>

### <a name="open-extension-limits"></a><span data-ttu-id="48594-231">Limites de extensão aberta</span><span class="sxs-lookup"><span data-stu-id="48594-231">Open extension limits</span></span>
<span data-ttu-id="48594-232">Os seguintes limites se aplicam aos recursos de diretório (como **usuário**, **grupo**, **dispositivo**):</span><span class="sxs-lookup"><span data-stu-id="48594-232">The following limits apply to directory resources (such as **user**, **group**, **device**):</span></span>

- <span data-ttu-id="48594-233">Cada extensão aberta pode ter até 2 KB de dados (incluindo a definição da extensão em si).</span><span class="sxs-lookup"><span data-stu-id="48594-233">Each open extension can have up to 2KB of data (including the extension definition itself).</span></span>
- <span data-ttu-id="48594-234">Um aplicativo pode adicionar até duas extensões abertas por instância do recurso.</span><span class="sxs-lookup"><span data-stu-id="48594-234">An application can add up to two open extensions per resource instance.</span></span>

### <a name="schema-extension-limits"></a><span data-ttu-id="48594-235">Limites de extensão do esquema</span><span class="sxs-lookup"><span data-stu-id="48594-235">Schema extension limits</span></span>
<span data-ttu-id="48594-236">Um aplicativo pode criar não mais de cinco definições de **extensão do esquema**.</span><span class="sxs-lookup"><span data-stu-id="48594-236">An application may create no more than five **schema extension** definitions.</span></span>

## <a name="known-limitations"></a><span data-ttu-id="48594-237">Limitações conhecidas</span><span class="sxs-lookup"><span data-stu-id="48594-237">Known limitations</span></span>

<span data-ttu-id="48594-238">Nas limitações conhecidas usando extensões, veja a [seção extensões](known_issues.md#extensions) no artigo problemas conhecidos.</span><span class="sxs-lookup"><span data-stu-id="48594-238">For known limitations using extensions, see the [extensions section](known_issues.md#extensions) in the known issues article.</span></span>

## <a name="extension-examples"></a><span data-ttu-id="48594-239">Exemplos de extensão</span><span class="sxs-lookup"><span data-stu-id="48594-239">Extension examples</span></span>

[<span data-ttu-id="48594-240">Adicionar dados personalizados aos usuários usando extensões abertas</span><span class="sxs-lookup"><span data-stu-id="48594-240">Add custom data to users using open extensions</span></span>](extensibility_open_users.md)

[<span data-ttu-id="48594-241">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="48594-241">Add custom data to groups using schema extensions</span></span>](extensibility_schema_groups.md)

## <a name="see-also"></a><span data-ttu-id="48594-242">Ver também</span><span class="sxs-lookup"><span data-stu-id="48594-242">See also</span></span>

[<span data-ttu-id="48594-243">Domínios do Office 365</span><span class="sxs-lookup"><span data-stu-id="48594-243">Office 365 domains</span></span>](https://technet.microsoft.com/en-us/library/office-365-domains.aspx)

[<span data-ttu-id="48594-244">Adição e verificação de um domínio para um locatário do Office 365</span><span class="sxs-lookup"><span data-stu-id="48594-244">Adding and verifying a domain for an Office 365 tenant</span></span>](http://office365support.ca/adding-and-verifying-a-domain-for-the-new-office-365/)
