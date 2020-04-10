---
title: Atualizar o servicePrincipalName
description: Atualiza as propriedades do objeto servicePrincipalName.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 072351ebc95d8610bc069055aacb0b193e1ca626
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218602"
---
# <a name="update-serviceprincipal"></a><span data-ttu-id="02c7f-103">Atualizar o servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="02c7f-103">Update serviceprincipal</span></span>

<span data-ttu-id="02c7f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02c7f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02c7f-105">Atualiza as propriedades do objeto servicePrincipalName.</span><span class="sxs-lookup"><span data-stu-id="02c7f-105">Update the properties of serviceprincipal object.</span></span>
## <a name="permissions"></a><span data-ttu-id="02c7f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="02c7f-106">Permissions</span></span>
<span data-ttu-id="02c7f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02c7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02c7f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02c7f-109">Permission type</span></span>      | <span data-ttu-id="02c7f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02c7f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02c7f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02c7f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="02c7f-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="02c7f-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="02c7f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02c7f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02c7f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02c7f-114">Not supported.</span></span>    |
|<span data-ttu-id="02c7f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02c7f-115">Application</span></span> | <span data-ttu-id="02c7f-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02c7f-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="02c7f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02c7f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a><span data-ttu-id="02c7f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02c7f-118">Request headers</span></span>
| <span data-ttu-id="02c7f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="02c7f-119">Name</span></span>       | <span data-ttu-id="02c7f-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="02c7f-120">Type</span></span> | <span data-ttu-id="02c7f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="02c7f-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="02c7f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="02c7f-122">Authorization</span></span>  | <span data-ttu-id="02c7f-123">string</span><span class="sxs-lookup"><span data-stu-id="02c7f-123">string</span></span>  | <span data-ttu-id="02c7f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02c7f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="02c7f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02c7f-126">Request body</span></span>
<span data-ttu-id="02c7f-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="02c7f-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="02c7f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02c7f-130">Property</span></span>     | <span data-ttu-id="02c7f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="02c7f-131">Type</span></span>   |<span data-ttu-id="02c7f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="02c7f-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02c7f-133">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="02c7f-133">accountEnabled</span></span>|<span data-ttu-id="02c7f-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="02c7f-134">Boolean</span></span>|                <span data-ttu-id="02c7f-135">**True** se a entidade de serviço estiver habilitada; caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="02c7f-135">**true** if the service principal account is enabled; otherwise, **false**.</span></span>            |
|<span data-ttu-id="02c7f-136">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="02c7f-136">appDisplayName</span></span>|<span data-ttu-id="02c7f-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02c7f-137">String</span></span>|<span data-ttu-id="02c7f-138">O nome de exibição exposto pelo aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="02c7f-138">The display name exposed by the associated application.</span></span>|
|<span data-ttu-id="02c7f-139">appId</span><span class="sxs-lookup"><span data-stu-id="02c7f-139">appId</span></span>|<span data-ttu-id="02c7f-140">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="02c7f-140">String</span></span>|<span data-ttu-id="02c7f-141">O identificador exclusivo do aplicativo associado (sua propriedade **appId**).</span><span class="sxs-lookup"><span data-stu-id="02c7f-141">The unique identifier for the associated application (its **appId** property).</span></span>|
|<span data-ttu-id="02c7f-142">appRoleAssignmentRequired</span><span class="sxs-lookup"><span data-stu-id="02c7f-142">appRoleAssignmentRequired</span></span>|<span data-ttu-id="02c7f-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="02c7f-143">Boolean</span></span>|<span data-ttu-id="02c7f-144">Especifica se um **appRoleAssignment** de um usuário ou grupo é necessário antes que o Azure AD emita um token de usuário ou de acesso ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="02c7f-144">Specifies whether an **appRoleAssignment** to a user or group is required before Azure AD will issue a user or access token to the application.</span></span>                            <span data-ttu-id="02c7f-145">**Observações**: requer a versão 1,5 ou posterior, não anulável.</span><span class="sxs-lookup"><span data-stu-id="02c7f-145">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="02c7f-146">appRoles</span><span class="sxs-lookup"><span data-stu-id="02c7f-146">appRoles</span></span>|<span data-ttu-id="02c7f-147">appRole</span><span class="sxs-lookup"><span data-stu-id="02c7f-147">appRole</span></span>|<span data-ttu-id="02c7f-148">As funções do aplicativo expostas pelo aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="02c7f-148">The application roles exposed by the associated application.</span></span> <span data-ttu-id="02c7f-149">Para obter mais informações, consulte a definição da propriedade **appRoles** na entidade de aplicativo **observações**: requer a versão 1,5 ou posterior, não anulável.</span><span class="sxs-lookup"><span data-stu-id="02c7f-149">For more information see the **appRoles** property definition on the application entity                            **Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="02c7f-150">displayName</span><span class="sxs-lookup"><span data-stu-id="02c7f-150">displayName</span></span>|<span data-ttu-id="02c7f-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02c7f-151">String</span></span>|<span data-ttu-id="02c7f-152">O nome de exibição da entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="02c7f-152">The display name for the service principal.</span></span>|
|<span data-ttu-id="02c7f-153">errorUrl</span><span class="sxs-lookup"><span data-stu-id="02c7f-153">errorUrl</span></span>|<span data-ttu-id="02c7f-154">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="02c7f-154">String</span></span>|            |
|<span data-ttu-id="02c7f-155">homepage</span><span class="sxs-lookup"><span data-stu-id="02c7f-155">homepage</span></span>|<span data-ttu-id="02c7f-156">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="02c7f-156">String</span></span>|<span data-ttu-id="02c7f-157">A URL da home page do aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="02c7f-157">The URL to the homepage of the associated application.</span></span>|
|<span data-ttu-id="02c7f-158">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="02c7f-158">keyCredentials</span></span>|<span data-ttu-id="02c7f-159">keycredential</span><span class="sxs-lookup"><span data-stu-id="02c7f-159">keyCredential</span></span>|<span data-ttu-id="02c7f-160">A coleção de credenciais principais associada à entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="02c7f-160">The collection of key credentials associated with the service principal.</span></span>                            <span data-ttu-id="02c7f-161">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="02c7f-161">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="02c7f-162">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="02c7f-162">logoutUrl</span></span>|<span data-ttu-id="02c7f-163">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="02c7f-163">String</span></span>| <span data-ttu-id="02c7f-164">Especifica a URL que será usada pela autorização do serviço da Microsoft para fazer logoff de um usuário usando protocolos de logoff [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) ou SAML.</span><span class="sxs-lookup"><span data-stu-id="02c7f-164">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="02c7f-165">oauth2Permissions</span><span class="sxs-lookup"><span data-stu-id="02c7f-165">oauth2Permissions</span></span>|<span data-ttu-id="02c7f-166">oAuth2Permission</span><span class="sxs-lookup"><span data-stu-id="02c7f-166">oAuth2Permission</span></span>|<span data-ttu-id="02c7f-167">As permissões OAuth 2.0 expostas pelo aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="02c7f-167">The OAuth 2.0 permissions exposed by the associated application.</span></span> <span data-ttu-id="02c7f-168">Para obter mais informações, confira a definição da propriedade **oauth2Permissions** na entidade aplicativo.</span><span class="sxs-lookup"><span data-stu-id="02c7f-168">For more information see the **oauth2Permissions** property definition on the application entity.</span></span>                            <span data-ttu-id="02c7f-169">**Observações**: requer a versão 1,5 ou posterior, não anulável.</span><span class="sxs-lookup"><span data-stu-id="02c7f-169">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="02c7f-170">passwordCredentials</span><span class="sxs-lookup"><span data-stu-id="02c7f-170">passwordCredentials</span></span>|<span data-ttu-id="02c7f-171">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="02c7f-171">passwordCredential</span></span>|<span data-ttu-id="02c7f-172">A coleção de credenciais de senha associada à entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="02c7f-172">The collection of password credentials associated with the service principal.</span></span>                            <span data-ttu-id="02c7f-173">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="02c7f-173">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="02c7f-174">preferredTokenSigningKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="02c7f-174">preferredTokenSigningKeyThumbprint</span></span>|<span data-ttu-id="02c7f-175">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="02c7f-175">String</span></span>|<span data-ttu-id="02c7f-176">Reservado apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="02c7f-176">Reserved for internal use only.</span></span> <span data-ttu-id="02c7f-177">Não escreva ou dependa de alguma forma dessa propriedade.</span><span class="sxs-lookup"><span data-stu-id="02c7f-177">Do not write or otherwise rely on this property.</span></span> <span data-ttu-id="02c7f-178">Pode ser removida em versões futuras.</span><span class="sxs-lookup"><span data-stu-id="02c7f-178">May be removed in future versions.</span></span>                            <span data-ttu-id="02c7f-179">**Observações**: requer a versão 1,5 ou mais recente.</span><span class="sxs-lookup"><span data-stu-id="02c7f-179">**Notes**: Requires version 1.5 or newer.</span></span>            |
|<span data-ttu-id="02c7f-180">publisherName</span><span class="sxs-lookup"><span data-stu-id="02c7f-180">publisherName</span></span>|<span data-ttu-id="02c7f-181">String</span><span class="sxs-lookup"><span data-stu-id="02c7f-181">String</span></span>|<span data-ttu-id="02c7f-182">O nome de exibição do locatário no qual o aplicativo associado está especificado.</span><span class="sxs-lookup"><span data-stu-id="02c7f-182">The display name of the tenant in which the associated application is specified.</span></span>|
|<span data-ttu-id="02c7f-183">replyUrls</span><span class="sxs-lookup"><span data-stu-id="02c7f-183">replyUrls</span></span>|<span data-ttu-id="02c7f-184">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="02c7f-184">String</span></span>|<span data-ttu-id="02c7f-185">As URLs às quais os tokens de usuário são enviados para entrar com aplicativo associado ou os URIs de redirecionamento aos quais os códigos de autorização do OAuth 2.0 e tokens de acesso são enviados para o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="02c7f-185">The URLs that user tokens are sent to for sign in with the associated application, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to for the associated application.</span></span>                            <span data-ttu-id="02c7f-186">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="02c7f-186">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="02c7f-187">samlMetadataUrl</span><span class="sxs-lookup"><span data-stu-id="02c7f-187">samlMetadataUrl</span></span>|<span data-ttu-id="02c7f-188">String</span><span class="sxs-lookup"><span data-stu-id="02c7f-188">String</span></span>|            |
|<span data-ttu-id="02c7f-189">servicePrincipalNames</span><span class="sxs-lookup"><span data-stu-id="02c7f-189">servicePrincipalNames</span></span>|<span data-ttu-id="02c7f-190">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="02c7f-190">String</span></span>|<span data-ttu-id="02c7f-191">Os URIs que identificam o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="02c7f-191">The URIs that identify the associated application.</span></span> <span data-ttu-id="02c7f-192">Para saber mais, confira [Objetos do aplicativo e objetos da entidade de serviço](https://msdn.microsoft.com/library/azure/dn132633.aspx).</span><span class="sxs-lookup"><span data-stu-id="02c7f-192">For more information see, [Application Objects and Service Principal Objects](https://msdn.microsoft.com/library/azure/dn132633.aspx).</span></span>                            <span data-ttu-id="02c7f-193">**Observações**: não nulos, o operador **any** é obrigatório para expressões de filtro em Propriedades de vários valores; para obter mais informações, consulte [supported queries, Filters, and paging Options](https://msdn.microsoft.com/library/azure/dn727074.aspx).</span><span class="sxs-lookup"><span data-stu-id="02c7f-193">**Notes**: not nullable, the **any** operator is required for filter expressions on multi-valued properties; for more information, see [Supported Queries, Filters, and Paging Options](https://msdn.microsoft.com/library/azure/dn727074.aspx).</span></span>            |
|<span data-ttu-id="02c7f-194">tags</span><span class="sxs-lookup"><span data-stu-id="02c7f-194">tags</span></span>|<span data-ttu-id="02c7f-195">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="02c7f-195">String</span></span>|                                        <span data-ttu-id="02c7f-196">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="02c7f-196">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="02c7f-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="02c7f-197">Response</span></span>

<span data-ttu-id="02c7f-198">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [servicePrincipalName](../resources/serviceprincipal.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02c7f-198">If successful, this method returns a `200 OK` response code and updated [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="02c7f-199">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02c7f-199">Example</span></span>
##### <a name="request"></a><span data-ttu-id="02c7f-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02c7f-200">Request</span></span>
<span data-ttu-id="02c7f-201">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02c7f-201">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="02c7f-202">HTTP</span><span class="sxs-lookup"><span data-stu-id="02c7f-202">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="02c7f-203">C#</span><span class="sxs-lookup"><span data-stu-id="02c7f-203">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02c7f-204">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02c7f-204">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02c7f-205">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02c7f-205">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="02c7f-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="02c7f-206">Response</span></span>
<span data-ttu-id="02c7f-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02c7f-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
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
<!--
{
  "type": "#page.annotation",
  "description": "Update serviceprincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
