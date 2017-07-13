<span data-ttu-id="d0a7c-p114">As relações entre um domínio e outros objetos no diretório como seus registros de verificação e de configuração de serviço expostas por meio de propriedades de navegação. Você pode ler essas relações ao direcionar essas propriedades de navegação em suas solicitações.</span><span class="sxs-lookup"><span data-stu-id="d0a7c-p114">Relationships between a domain and other objects in the directory such as its verification records and service configuration records are exposed through navigation properties. You can read these relationships by targeting these navigation properties in your requests.</span></span>

As relações entre um domínio e outros objetos no diretório como seus registros de verificação e de configuração de serviço expostas por meio de propriedades de navegação. Você pode ler essas relações ao direcionar essas propriedades de navegação em suas solicitações.

| <span data-ttu-id="d0a7c-199">Relação</span><span class="sxs-lookup"><span data-stu-id="d0a7c-199">Relationship</span></span> | <span data-ttu-id="d0a7c-200">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0a7c-200">Type</span></span> |<span data-ttu-id="d0a7c-201">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0a7c-201">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0a7c-202">domainNameReferences</span><span class="sxs-lookup"><span data-stu-id="d0a7c-202">domainNameReferences</span></span>|<span data-ttu-id="d0a7c-203">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="d0a7c-203">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="d0a7c-204">Somente leitura, Anulável</span><span class="sxs-lookup"><span data-stu-id="d0a7c-204">Read-only, Nullable</span></span>|
|<span data-ttu-id="d0a7c-205">serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="d0a7c-205">serviceConfigurationRecords</span></span>|<span data-ttu-id="d0a7c-206">Coleção [domainDnsRecord](domaindnsrecord.md)</span><span class="sxs-lookup"><span data-stu-id="d0a7c-206">[domainDnsRecord](domaindnsrecord.md) collection</span></span>| <span data-ttu-id="d0a7c-207">Os registros DNS que o cliente adiciona ao arquivo de zona DNS do domínio antes que o domínio possa ser usado pelo Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="d0a7c-207">DNS records the customer adds to the DNS zone file of the domain before the domain can be used by Microsoft Online services.</span></span><br><span data-ttu-id="d0a7c-208">Somente leitura, Anulável</span><span class="sxs-lookup"><span data-stu-id="d0a7c-208">Read-only, Nullable</span></span> |
|<span data-ttu-id="d0a7c-209">verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="d0a7c-209">verificationDnsRecords</span></span>|<span data-ttu-id="d0a7c-210">Coleção [domainDnsRecord](domaindnsrecord.md)</span><span class="sxs-lookup"><span data-stu-id="d0a7c-210">[domainDnsRecord](domaindnsrecord.md) collection</span></span>| <span data-ttu-id="d0a7c-211">Os registros DNS que o cliente adiciona ao arquivo de zona DNS do domínio para que o cliente possa concluir a verificação de propriedade de domínio com o Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d0a7c-211">DNS records that the customer adds to the DNS zone file of the domain before the customer can complete domain ownership verification with Azure AD.</span></span><br><span data-ttu-id="d0a7c-212">Somente leitura, Anulável</span><span class="sxs-lookup"><span data-stu-id="d0a7c-212">Read-only, Nullable</span></span>|

## <span data-ttu-id="d0a7c-213">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d0a7c-213">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="d0a7c-214">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d0a7c-214">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domain"
}-->

```json
{
  "authenticationType": "String",
  "availabilityStatus": "String",
  "id": "String (identifier)",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "isVerified": true,
  "state": {"@odata.type": "microsoft.graph.domainState"},
  "supportedServices": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->