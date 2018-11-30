---
title: Atualizar serviceprincipal
description: Atualize as propriedades do objeto serviceprincipal.
ms.openlocfilehash: a24a8c949d48f577a3d7fe6208a1422819772801
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040666"
---
# <a name="update-serviceprincipal"></a><span data-ttu-id="82a89-103">Atualizar serviceprincipal</span><span class="sxs-lookup"><span data-stu-id="82a89-103">Update serviceprincipal</span></span>

> <span data-ttu-id="82a89-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="82a89-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="82a89-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="82a89-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="82a89-106">Atualize as propriedades do objeto serviceprincipal.</span><span class="sxs-lookup"><span data-stu-id="82a89-106">Update the properties of serviceprincipal object.</span></span>
## <a name="permissions"></a><span data-ttu-id="82a89-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="82a89-107">Permissions</span></span>
<span data-ttu-id="82a89-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82a89-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82a89-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="82a89-110">Permission type</span></span>      | <span data-ttu-id="82a89-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="82a89-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82a89-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="82a89-112">Delegated (work or school account)</span></span> | <span data-ttu-id="82a89-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="82a89-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="82a89-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="82a89-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82a89-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82a89-115">Not supported.</span></span>    |
|<span data-ttu-id="82a89-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="82a89-116">Application</span></span> | <span data-ttu-id="82a89-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82a89-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="82a89-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="82a89-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a><span data-ttu-id="82a89-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="82a89-119">Request headers</span></span>
| <span data-ttu-id="82a89-120">Nome</span><span class="sxs-lookup"><span data-stu-id="82a89-120">Name</span></span>       | <span data-ttu-id="82a89-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="82a89-121">Type</span></span> | <span data-ttu-id="82a89-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="82a89-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="82a89-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="82a89-123">Authorization</span></span>  | <span data-ttu-id="82a89-124">string</span><span class="sxs-lookup"><span data-stu-id="82a89-124">string</span></span>  | <span data-ttu-id="82a89-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82a89-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="82a89-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="82a89-127">Request body</span></span>
<span data-ttu-id="82a89-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="82a89-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="82a89-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82a89-131">Property</span></span>     | <span data-ttu-id="82a89-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="82a89-132">Type</span></span>   |<span data-ttu-id="82a89-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="82a89-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82a89-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="82a89-134">accountEnabled</span></span>|<span data-ttu-id="82a89-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="82a89-135">Boolean</span></span>|                <span data-ttu-id="82a89-136">**true** se a conta de serviço principal estiver ativada; Caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="82a89-136">**true** if the service principal account is enabled; otherwise, **false**.</span></span>            |
|<span data-ttu-id="82a89-137">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="82a89-137">appDisplayName</span></span>|<span data-ttu-id="82a89-138">String</span><span class="sxs-lookup"><span data-stu-id="82a89-138">String</span></span>|<span data-ttu-id="82a89-139">O nome de exibição exposto pelo aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="82a89-139">The display name exposed by the associated application.</span></span>|
|<span data-ttu-id="82a89-140">appId</span><span class="sxs-lookup"><span data-stu-id="82a89-140">appId</span></span>|<span data-ttu-id="82a89-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82a89-141">String</span></span>|<span data-ttu-id="82a89-142">O identificador exclusivo para o aplicativo associado (sua propriedade **appId** ).</span><span class="sxs-lookup"><span data-stu-id="82a89-142">The unique identifier for the associated application (its **appId** property).</span></span>|
|<span data-ttu-id="82a89-143">appRoleAssignmentRequired</span><span class="sxs-lookup"><span data-stu-id="82a89-143">appRoleAssignmentRequired</span></span>|<span data-ttu-id="82a89-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="82a89-144">Boolean</span></span>|<span data-ttu-id="82a89-145">Especifica se um **appRoleAssignment** a um usuário ou grupo é necessária antes que o Azure AD emitirá um usuário ou um token de acesso ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="82a89-145">Specifies whether an **appRoleAssignment** to a user or group is required before Azure AD will issue a user or access token to the application.</span></span>                            <span data-ttu-id="82a89-146">**Observações**: requer a versão 1.5 ou mais recente, não são nulas.</span><span class="sxs-lookup"><span data-stu-id="82a89-146">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="82a89-147">appRoles</span><span class="sxs-lookup"><span data-stu-id="82a89-147">appRoles</span></span>|<span data-ttu-id="82a89-148">appRole</span><span class="sxs-lookup"><span data-stu-id="82a89-148">appRole</span></span>|<span data-ttu-id="82a89-149">As funções do aplicativo expostas pelo aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="82a89-149">The application roles exposed by the associated application.</span></span> <span data-ttu-id="82a89-150">Para obter mais informações, consulte a definição da propriedade **appRoles** sobre a entidade de aplicativo **Notes**: requer a versão 1.5 ou mais recente, não são nulas.</span><span class="sxs-lookup"><span data-stu-id="82a89-150">For more information see the **appRoles** property definition on the application entity                            **Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="82a89-151">displayName</span><span class="sxs-lookup"><span data-stu-id="82a89-151">displayName</span></span>|<span data-ttu-id="82a89-152">String</span><span class="sxs-lookup"><span data-stu-id="82a89-152">String</span></span>|<span data-ttu-id="82a89-153">O nome de exibição para a entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="82a89-153">The display name for the service principal.</span></span>|
|<span data-ttu-id="82a89-154">errorUrl</span><span class="sxs-lookup"><span data-stu-id="82a89-154">errorUrl</span></span>|<span data-ttu-id="82a89-155">String</span><span class="sxs-lookup"><span data-stu-id="82a89-155">String</span></span>|            |
|<span data-ttu-id="82a89-156">home page</span><span class="sxs-lookup"><span data-stu-id="82a89-156">homepage</span></span>|<span data-ttu-id="82a89-157">String</span><span class="sxs-lookup"><span data-stu-id="82a89-157">String</span></span>|<span data-ttu-id="82a89-158">A URL para a home page do aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="82a89-158">The URL to the homepage of the associated application.</span></span>|
|<span data-ttu-id="82a89-159">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="82a89-159">keyCredentials</span></span>|<span data-ttu-id="82a89-160">keyCredential</span><span class="sxs-lookup"><span data-stu-id="82a89-160">keyCredential</span></span>|<span data-ttu-id="82a89-161">A coleção de credenciais de chave associado ao serviço principal.</span><span class="sxs-lookup"><span data-stu-id="82a89-161">The collection of key credentials associated with the service principal.</span></span>                            <span data-ttu-id="82a89-162">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="82a89-162">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="82a89-163">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="82a89-163">logoutUrl</span></span>|<span data-ttu-id="82a89-164">String</span><span class="sxs-lookup"><span data-stu-id="82a89-164">String</span></span>| <span data-ttu-id="82a89-165">Especifica a URL que será usada pelo serviço de autorização da Microsoft para logout um usuário usando o [canal de frente](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) ou protocolos de logout SAML.</span><span class="sxs-lookup"><span data-stu-id="82a89-165">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="82a89-166">oauth2Permissions</span><span class="sxs-lookup"><span data-stu-id="82a89-166">oauth2Permissions</span></span>|<span data-ttu-id="82a89-167">oAuth2Permission</span><span class="sxs-lookup"><span data-stu-id="82a89-167">oAuth2Permission</span></span>|<span data-ttu-id="82a89-168">As permissões de OAuth 2.0 expostas pelo aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="82a89-168">The OAuth 2.0 permissions exposed by the associated application.</span></span> <span data-ttu-id="82a89-169">Para obter mais informações, consulte a definição da propriedade **oauth2Permissions** sobre a entidade de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="82a89-169">For more information see the **oauth2Permissions** property definition on the application entity.</span></span>                            <span data-ttu-id="82a89-170">**Observações**: requer a versão 1.5 ou mais recente, não são nulas.</span><span class="sxs-lookup"><span data-stu-id="82a89-170">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="82a89-171">passwordCredentials</span><span class="sxs-lookup"><span data-stu-id="82a89-171">passwordCredentials</span></span>|<span data-ttu-id="82a89-172">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="82a89-172">passwordCredential</span></span>|<span data-ttu-id="82a89-173">A coleção de credenciais de senha associadas a entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="82a89-173">The collection of password credentials associated with the service principal.</span></span>                            <span data-ttu-id="82a89-174">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="82a89-174">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="82a89-175">preferredTokenSigningKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="82a89-175">preferredTokenSigningKeyThumbprint</span></span>|<span data-ttu-id="82a89-176">String</span><span class="sxs-lookup"><span data-stu-id="82a89-176">String</span></span>|<span data-ttu-id="82a89-177">Reservado para uso interno apenas.</span><span class="sxs-lookup"><span data-stu-id="82a89-177">Reserved for internal use only.</span></span> <span data-ttu-id="82a89-178">Não gravar ou caso contrário, contam com esta propriedade.</span><span class="sxs-lookup"><span data-stu-id="82a89-178">Do not write or otherwise rely on this property.</span></span> <span data-ttu-id="82a89-179">Pode ser removido em futuras versões.</span><span class="sxs-lookup"><span data-stu-id="82a89-179">May be removed in future versions.</span></span>                            <span data-ttu-id="82a89-180">**Observações**: requer a versão 1.5 ou mais recente.</span><span class="sxs-lookup"><span data-stu-id="82a89-180">**Notes**: Requires version 1.5 or newer.</span></span>            |
|<span data-ttu-id="82a89-181">publisherName</span><span class="sxs-lookup"><span data-stu-id="82a89-181">publisherName</span></span>|<span data-ttu-id="82a89-182">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82a89-182">String</span></span>|<span data-ttu-id="82a89-183">O nome de exibição do inquilino no qual o aplicativo associado for especificado.</span><span class="sxs-lookup"><span data-stu-id="82a89-183">The display name of the tenant in which the associated application is specified.</span></span>|
|<span data-ttu-id="82a89-184">replyUrls</span><span class="sxs-lookup"><span data-stu-id="82a89-184">replyUrls</span></span>|<span data-ttu-id="82a89-185">String</span><span class="sxs-lookup"><span data-stu-id="82a89-185">String</span></span>|<span data-ttu-id="82a89-186">As URLs que os tokens do usuário são enviados para entrada com o aplicativo associado ou o redirecionamento códigos de autorização de URIs que OAuth 2.0 e tokens de acesso são enviados para o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="82a89-186">The URLs that user tokens are sent to for sign in with the associated application, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to for the associated application.</span></span>                            <span data-ttu-id="82a89-187">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="82a89-187">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="82a89-188">samlMetadataUrl</span><span class="sxs-lookup"><span data-stu-id="82a89-188">samlMetadataUrl</span></span>|<span data-ttu-id="82a89-189">String</span><span class="sxs-lookup"><span data-stu-id="82a89-189">String</span></span>|            |
|<span data-ttu-id="82a89-190">servicePrincipalNames</span><span class="sxs-lookup"><span data-stu-id="82a89-190">servicePrincipalNames</span></span>|<span data-ttu-id="82a89-191">String</span><span class="sxs-lookup"><span data-stu-id="82a89-191">String</span></span>|<span data-ttu-id="82a89-192">Os URIs que identificam o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="82a89-192">The URIs that identify the associated application.</span></span> <span data-ttu-id="82a89-193">Para mais informações, consulte [objetos de aplicativo e objetos de entidade de serviço](https://msdn.microsoft.com/library/azure/dn132633.aspx).</span><span class="sxs-lookup"><span data-stu-id="82a89-193">For more information see, [Application Objects and Service Principal Objects](https://msdn.microsoft.com/library/azure/dn132633.aspx).</span></span>                            <span data-ttu-id="82a89-194">**Observações**: não são nulas, o operador **any** é necessário para expressões de filtro propriedades de valores múltiplos; Para obter mais informações, consulte [suporte para consultas, filtros e opções de paginação](https://msdn.microsoft.com/library/azure/dn727074.aspx).</span><span class="sxs-lookup"><span data-stu-id="82a89-194">**Notes**: not nullable, the **any** operator is required for filter expressions on multi-valued properties; for more information, see [Supported Queries, Filters, and Paging Options](https://msdn.microsoft.com/library/azure/dn727074.aspx).</span></span>            |
|<span data-ttu-id="82a89-195">marcas</span><span class="sxs-lookup"><span data-stu-id="82a89-195">tags</span></span>|<span data-ttu-id="82a89-196">String</span><span class="sxs-lookup"><span data-stu-id="82a89-196">String</span></span>|                                        <span data-ttu-id="82a89-197">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="82a89-197">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="82a89-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="82a89-198">Response</span></span>

<span data-ttu-id="82a89-199">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto atualizado [servicePrincipal](../resources/serviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="82a89-199">If successful, this method returns a `200 OK` response code and updated [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="82a89-200">Exemplo</span><span class="sxs-lookup"><span data-stu-id="82a89-200">Example</span></span>
##### <a name="request"></a><span data-ttu-id="82a89-201">Solicitação</span><span class="sxs-lookup"><span data-stu-id="82a89-201">Request</span></span>
<span data-ttu-id="82a89-202">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="82a89-202">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_serviceprincipal"
}-->
```http
PATCH https://graph.microsoft.com/beta/servicePrincipals/{id}
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
```
##### <a name="response"></a><span data-ttu-id="82a89-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="82a89-203">Response</span></span>
<span data-ttu-id="82a89-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="82a89-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceprincipal"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update serviceprincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
