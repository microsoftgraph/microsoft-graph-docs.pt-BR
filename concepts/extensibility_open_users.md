<span data-ttu-id="71265-p107">O usuário decide que, se não quiser mais um perfil móvel, pode excluí-lo. Esta atualização pode ser feita com uma solicitação ```DELETE``` no valor extensão aberto.</span><span class="sxs-lookup"><span data-stu-id="71265-p107">The user decides that they don't want a roaming profile anymore, so they delete it. This can be done with a ```DELETE``` request on the open extension value.</span></span>
O usuário decide que, se não quiser mais um perfil móvel, pode excluí-lo. Esta atualização pode ser feita com uma solicitação ```DELETE``` no valor extensão aberto.

##### <a name="request"></a><span data-ttu-id="71265-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71265-135">Request</span></span>
```http
DELETE https://graph.microsoft.com/v1.0/me/extensions/com.contoso.roamingSettings
```

##### <a name="response"></a><span data-ttu-id="71265-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="71265-136">Response</span></span>
```
HTTP/1.1 204 No content
```

## <a name="see-also"></a><span data-ttu-id="71265-137">Ver também</span><span class="sxs-lookup"><span data-stu-id="71265-137">See also</span></span>

- [<span data-ttu-id="71265-138">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="71265-138">Add custom data to resources using extensions</span></span>](extensibility_overview.md)
- [<span data-ttu-id="71265-139">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="71265-139">Add custom data to groups using schema extensions</span></span>](extensibility_schema_groups.md)
- [<span data-ttu-id="71265-140">tipo de recurso openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="71265-140">openTypeExtension resource type</span></span>](../api-reference/v1.0/resources/opentypeextension.md)
- [<span data-ttu-id="71265-141">Criar extensão aberta</span><span class="sxs-lookup"><span data-stu-id="71265-141">Create open extension</span></span>](../api-reference/v1.0/api/opentypeextension_post_opentypeextension.md)
- [<span data-ttu-id="71265-142">Obter extensão aberta</span><span class="sxs-lookup"><span data-stu-id="71265-142">Get open extension</span></span>](../api-reference/v1.0/api/opentypeextension_get.md)
- [<span data-ttu-id="71265-143">Atualizar extensão aberta</span><span class="sxs-lookup"><span data-stu-id="71265-143">Update open extension</span></span>](../api-reference/v1.0/api/opentypeextension_update.md)
- [<span data-ttu-id="71265-144">Excluir extensão aberta</span><span class="sxs-lookup"><span data-stu-id="71265-144">Delete open extension</span></span>](../api-reference/v1.0/api/opentypeextension_delete.md)