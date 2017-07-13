<span data-ttu-id="eae3b-p109">O exemplo a seguir procura o grupo que possui a extensão `graphlearn_courses` com um valor de propriedade `courseId` correspondente a `123` e obtém as propriedades do grupo **displayName**, **id** e **description** e os dados personalizados na extensão `graphlearn_courses`. (Na consulta em si, certifique-se de aplicar codificação de URL conforme necessário).</span><span class="sxs-lookup"><span data-stu-id="eae3b-p109">The following example looks for the group that has the `graphlearn_courses` extension with a `courseId` property value matching `123`, and gets the group properties **displayName**, **id**, and **description**, and the custom data in the `graphlearn_courses` extension. (In the actual query, make sure you apply URL encoding as necessary.)</span></span>

O exemplo a seguir procura o grupo que possui a extensão `graphlearn_courses` com um valor de propriedade `courseId` correspondente a `123` e obtém as propriedades do grupo **displayName**, **id** e **description** e os dados personalizados na extensão `graphlearn_courses`. (Na consulta em si, certifique-se de aplicar codificação de URL conforme necessário).

#### <span data-ttu-id="eae3b-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eae3b-157">Request</span></span>
<a id="request" class="xliff"></a>

```http
GET https://graph.microsoft.com/v1.0/groups?$filter=graphlearn_courses/courseId eq ‘123’&$select=displayName,id,description,graphlearn_courses
```


##### <span data-ttu-id="eae3b-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="eae3b-158">Response</span></span>
<a id="response" class="xliff"></a>
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 326
{
  "value": [
    {
      "displayName": "New Managers March 2017",
      "id": "14429ae5-3e74-41a2-9fa8-028fbb984637",
      "description": "New Managers training course for March 2017",
      "graphlearn_courses": {
        "@odata.type": "#microsoft.graph.ComplexExtensionValue",
        "courseId":"123",
        "courseName":"New Managers",
        "courseType":"Online"
      }
    }
  ]
}
```

## <span data-ttu-id="eae3b-159">Ver também</span><span class="sxs-lookup"><span data-stu-id="eae3b-159">See also</span></span>
<a id="see-also" class="xliff"></a>

- [<span data-ttu-id="eae3b-160">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="eae3b-160">Add custom data to resources using extensions</span></span>](extensibility_overview.md)
- [<span data-ttu-id="eae3b-161">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="eae3b-161">Add custom data to users using open extensions (preview)</span></span>](extensibility_open_users.md)
- <span data-ttu-id="eae3b-162">
  [Domínios do Office 365](https://technet.microsoft.com/en-us/library/office-365-domains.aspx)</span><span class="sxs-lookup"><span data-stu-id="eae3b-162">[Office 365 domains](https://technet.microsoft.com/en-us/library/office-365-domains.aspx)</span></span>
- [<span data-ttu-id="eae3b-163">Adicionando e verificando um domínio para o NOVO Office 365</span><span class="sxs-lookup"><span data-stu-id="eae3b-163">Adding and Verifying a Domain for the NEW Office 365</span></span>](http://office365support.ca/adding-and-verifying-a-domain-for-the-new-office-365/)
- [<span data-ttu-id="eae3b-164">Tipo de recurso schemaExtension</span><span class="sxs-lookup"><span data-stu-id="eae3b-164">schemaExtension resource type</span></span>](../api-reference/v1.0/resources/schemaextension.md)
- [<span data-ttu-id="eae3b-165">List schemaExtensions</span><span class="sxs-lookup"><span data-stu-id="eae3b-165">List schemaExtensions</span></span>](../api-reference/v1.0/api/schemaextension_list.md)
- [<span data-ttu-id="eae3b-166">Create schemaExtension</span><span class="sxs-lookup"><span data-stu-id="eae3b-166">Create schemaExtension</span></span>](../api-reference/v1.0/api/schemaextension_post_schemaextensions.md)
- [<span data-ttu-id="eae3b-167">Get schemaExtension</span><span class="sxs-lookup"><span data-stu-id="eae3b-167">Get schemaExtension</span></span>](../api-reference/v1.0/api/schemaextension_get.md)
- [<span data-ttu-id="eae3b-168">Update schemaExtension</span><span class="sxs-lookup"><span data-stu-id="eae3b-168">Update schemaExtension</span></span>](../api-reference/v1.0/api/schemaextension_update.md)
- [<span data-ttu-id="eae3b-169">Delete schemaExtension</span><span class="sxs-lookup"><span data-stu-id="eae3b-169">Delete schemaExtension</span></span>](../api-reference/v1.0/api/schemaextension_delete.md)
