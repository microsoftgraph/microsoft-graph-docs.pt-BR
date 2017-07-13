<span data-ttu-id="324c8-p107">O conjunto de tipos do Microsoft Graph (que podem suportar extensões) ao qual a extensão de esquema pode ser aplicada.  Somente as alterações aditivas são permitidas.</span><span class="sxs-lookup"><span data-stu-id="324c8-p107">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.  Only additive changes are permitted.</span></span>|O conjunto de tipos do Microsoft Graph (que podem suportar extensões) ao qual a extensão de esquema pode ser aplicada.  Somente as alterações aditivas são permitidas.|

## <span data-ttu-id="324c8-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="324c8-142">Response</span></span>
<a id="response" class="xliff"></a>

<span data-ttu-id="324c8-143">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="324c8-143">If successful, this method returns a `204 No Content` response code.</span></span>

## <span data-ttu-id="324c8-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="324c8-144">Example</span></span>
<a id="example" class="xliff"></a>

##### <span data-ttu-id="324c8-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="324c8-145">Request</span></span>
<a id="request" class="xliff"></a>

<span data-ttu-id="324c8-146">Veja a seguir um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="324c8-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/schemaExtensions/{id}
Content-type: application/json
Content-length: 201

{
  "properties": [
    {
      "name":"new-name-value",
      "type":"new-type-value"
    },
    {
      "name":"additional-name-value",
      "type":"additional-type-value"
    }
  ],
}
```

##### <span data-ttu-id="324c8-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="324c8-147">Response</span></span>
<a id="response" class="xliff"></a>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 204 No Content
```

## <span data-ttu-id="324c8-148">Ver também</span><span class="sxs-lookup"><span data-stu-id="324c8-148">See also</span></span>
<a id="see-also" class="xliff"></a>

- [<span data-ttu-id="324c8-149">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="324c8-149">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="324c8-150">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="324c8-150">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->