---
title: Atualizar serviceprincipal
description: Atualizar as propriedades do objeto serviceprincipal.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 82e936f93c10acb6e63672faac08653373f45fe6
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787123"
---
# <a name="update-serviceprincipal"></a><span data-ttu-id="7a896-103">Atualizar servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="7a896-103">Update servicePrincipal</span></span>

<span data-ttu-id="7a896-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a896-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7a896-105">Atualizar as propriedades do objeto [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="7a896-105">Update the properties of [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="7a896-106">Não há suporte para o uso do PATCH para definir [**passwordCredential**](../resources/passwordcredential.md).</span><span class="sxs-lookup"><span data-stu-id="7a896-106">Using PATCH to set [**passwordCredential**](../resources/passwordcredential.md) is not supported.</span></span> <span data-ttu-id="7a896-107">Use os métodos [addPassword](./serviceprincipal-addpassword.md) e [removePassword](./serviceprincipal-removepassword.md) para atualizá-la para uma entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="7a896-107">Use the [addPassword](./serviceprincipal-addpassword.md) and [removePassword](./serviceprincipal-removepassword.md) methods to update the password for a servicePrincipal.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a896-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="7a896-108">Permissions</span></span>
<span data-ttu-id="7a896-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a896-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a896-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a896-111">Permission type</span></span>      | <span data-ttu-id="7a896-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7a896-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a896-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a896-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7a896-114">Application.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7a896-114">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7a896-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a896-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a896-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a896-116">Not supported.</span></span>    |
|<span data-ttu-id="7a896-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a896-117">Application</span></span> | <span data-ttu-id="7a896-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a896-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a896-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a896-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7a896-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a896-120">Request headers</span></span>
| <span data-ttu-id="7a896-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7a896-121">Name</span></span>       | <span data-ttu-id="7a896-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a896-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="7a896-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a896-123">Authorization</span></span> | <span data-ttu-id="7a896-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a896-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7a896-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7a896-126">Content-Type</span></span> | <span data-ttu-id="7a896-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a896-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7a896-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a896-129">Request body</span></span>
<span data-ttu-id="7a896-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="7a896-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7a896-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a896-133">Property</span></span>     | <span data-ttu-id="7a896-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a896-134">Type</span></span> |<span data-ttu-id="7a896-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a896-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a896-136">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="7a896-136">accountEnabled</span></span>|<span data-ttu-id="7a896-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a896-137">Boolean</span></span>| <span data-ttu-id="7a896-138">**True** se a entidade de serviço estiver habilitada; caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="7a896-138">**true** if the service principal account is enabled; otherwise, **false**.</span></span>|
|<span data-ttu-id="7a896-139">addIns</span><span class="sxs-lookup"><span data-stu-id="7a896-139">addIns</span></span>| [<span data-ttu-id="7a896-140">addIn</span><span class="sxs-lookup"><span data-stu-id="7a896-140">addIn</span></span>](../resources/addin.md) | <span data-ttu-id="7a896-141">Define o comportamento personalizado que um serviço de consumo pode usar para chamar um aplicativo em contextos específicos.</span><span class="sxs-lookup"><span data-stu-id="7a896-141">Defines custom behavior that a consuming service can use to call an app in specific contexts.</span></span> <span data-ttu-id="7a896-142">Por exemplo, aplicativos que podem renderizar fluxos de arquivo [podem definir a propriedade addIns](/onedrive/developer/file-handlers/?view=odsp-graph-online) para a funcionalidade "FileHandler".</span><span class="sxs-lookup"><span data-stu-id="7a896-142">For example, applications that can render file streams [may set the addIns property](/onedrive/developer/file-handlers/?view=odsp-graph-online) for its "FileHandler" functionality.</span></span> <span data-ttu-id="7a896-143">Isso permitirá que os serviços como o Microsoft 365 chamem o aplicativo no contexto de um documento no qual o usuário esteja trabalhando.</span><span class="sxs-lookup"><span data-stu-id="7a896-143">This will let services like Microsoft 365 call the application in the context of a document the user is working on.</span></span>|
|<span data-ttu-id="7a896-144">alternativeNames</span><span class="sxs-lookup"><span data-stu-id="7a896-144">alternativeNames</span></span>|<span data-ttu-id="7a896-145">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a896-145">String collection</span></span>| <span data-ttu-id="7a896-146">Usado para recuperar entidades de serviço por assinatura, identificar grupo de recursos e IDs de recursos completos de [identidades gerenciadas](https://aka.ms/azuremanagedidentity).</span><span class="sxs-lookup"><span data-stu-id="7a896-146">Used to retrieve service principals by subscription, identify resource group and full resource ids for [managed identities](https://aka.ms/azuremanagedidentity).</span></span>|
|<span data-ttu-id="7a896-147">appRoleAssignmentRequired</span><span class="sxs-lookup"><span data-stu-id="7a896-147">appRoleAssignmentRequired</span></span>|<span data-ttu-id="7a896-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a896-148">Boolean</span></span>|<span data-ttu-id="7a896-149">Especifica se um **appRoleAssignment** de um usuário ou grupo é necessário antes que o Azure AD emita um token de usuário ou de acesso ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7a896-149">Specifies whether an **appRoleAssignment** to a user or group is required before Azure AD will issue a user or access token to the application.</span></span> <span data-ttu-id="7a896-150">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="7a896-150">Not nullable.</span></span> |
|<span data-ttu-id="7a896-151">appRoles</span><span class="sxs-lookup"><span data-stu-id="7a896-151">appRoles</span></span>|<span data-ttu-id="7a896-152">[appRole](../resources/approle.md) collection</span><span class="sxs-lookup"><span data-stu-id="7a896-152">[appRole](../resources/approle.md) collection</span></span>|<span data-ttu-id="7a896-153">As funções do aplicativo expostas pelo aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="7a896-153">The application roles exposed by the associated application.</span></span> <span data-ttu-id="7a896-154">Para obter mais informações, confira a definição da propriedade **appRoles** no recurso [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="7a896-154">For more information see the **appRoles** property definition on the [application](../resources/application.md) resource.</span></span> <span data-ttu-id="7a896-155">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="7a896-155">Not nullable.</span></span> |
|<span data-ttu-id="7a896-156">displayName</span><span class="sxs-lookup"><span data-stu-id="7a896-156">displayName</span></span>|<span data-ttu-id="7a896-157">String</span><span class="sxs-lookup"><span data-stu-id="7a896-157">String</span></span>|<span data-ttu-id="7a896-158">O nome de exibição da entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="7a896-158">The display name for the service principal.</span></span>|
|<span data-ttu-id="7a896-159">homepage</span><span class="sxs-lookup"><span data-stu-id="7a896-159">homepage</span></span>|<span data-ttu-id="7a896-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a896-160">String</span></span>|<span data-ttu-id="7a896-161">Página inicial ou página de aterrissagem do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7a896-161">Home page or landing page of the application.</span></span>|
|<span data-ttu-id="7a896-162">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="7a896-162">keyCredentials</span></span>|<span data-ttu-id="7a896-163">[keyCredential](../resources/keycredential.md) collection</span><span class="sxs-lookup"><span data-stu-id="7a896-163">[keyCredential](../resources/keycredential.md) collection</span></span>|<span data-ttu-id="7a896-p109">A coleta de principais credenciais associadas ao diretor de serviços. Não pode ser anulado.</span><span class="sxs-lookup"><span data-stu-id="7a896-p109">The collection of key credentials associated with the service principal. Not nullable.</span></span>            |
|<span data-ttu-id="7a896-166">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="7a896-166">logoutUrl</span></span>|<span data-ttu-id="7a896-167">String</span><span class="sxs-lookup"><span data-stu-id="7a896-167">String</span></span>| <span data-ttu-id="7a896-168">Especifica a URL que será usada pela autorização do serviço da Microsoft para fazer logoff de um usuário usando protocolos de logoff [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) ou SAML.</span><span class="sxs-lookup"><span data-stu-id="7a896-168">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span>|
|<span data-ttu-id="7a896-169">oauth2PermissionScopes</span><span class="sxs-lookup"><span data-stu-id="7a896-169">oauth2PermissionScopes</span></span>|<span data-ttu-id="7a896-170">coleção [permissionScope](../resources/permissionScope.md)</span><span class="sxs-lookup"><span data-stu-id="7a896-170">[permissionScope](../resources/permissionScope.md) collection</span></span>|<span data-ttu-id="7a896-171">As permissões do escopo OAuth 2.0 expostas pelo aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="7a896-171">The OAuth 2.0 permission scopes exposed by the associated application.</span></span> <span data-ttu-id="7a896-172">Para obter mais informações, confira a definição da propriedade **oauth2PermissionScopes** no recurso [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="7a896-172">For more information see the **oauth2PermissionScopes** property definition on the [application](../resources/application.md) resource.</span></span> <span data-ttu-id="7a896-173">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="7a896-173">Not nullable.</span></span>|
|<span data-ttu-id="7a896-174">preferredSingleSignOnMode</span><span class="sxs-lookup"><span data-stu-id="7a896-174">preferredSingleSignOnMode</span></span>|<span data-ttu-id="7a896-175">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a896-175">string</span></span>|<span data-ttu-id="7a896-176">Especifica o modo de logon único configurado para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7a896-176">Specifies the single sign-on mode configured for this application.</span></span> <span data-ttu-id="7a896-177">O Azure AD usa o modo de logon único preferido para iniciar o aplicativo do Microsoft 365 ou o Azure AD My Apps.</span><span class="sxs-lookup"><span data-stu-id="7a896-177">Azure AD uses the preferred single sign-on mode to launch the application from Microsoft 365 or the Azure AD My Apps.</span></span> <span data-ttu-id="7a896-178">Os valores com suporte são: `password`, `saml`, `external`, e `oidc`.</span><span class="sxs-lookup"><span data-stu-id="7a896-178">The supported values are `password`, `saml`, `external`, and `oidc`.</span></span>|
|<span data-ttu-id="7a896-179">replyUrls</span><span class="sxs-lookup"><span data-stu-id="7a896-179">replyUrls</span></span>|<span data-ttu-id="7a896-180">String collection</span><span class="sxs-lookup"><span data-stu-id="7a896-180">String collection</span></span>|<span data-ttu-id="7a896-p112">URLs para as quais os tokens de usuário são enviados para se conectar com a aplicação associada, ou as URIs redirecionadas para as quais os códigos de autorização OAuth 2.0 e os tokens de acesso são enviados para a aplicação associada. Não pode ser anulado.</span><span class="sxs-lookup"><span data-stu-id="7a896-p112">The URLs that user tokens are sent to for sign in with the associated application, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to for the associated application. Not nullable.</span></span> |
|<span data-ttu-id="7a896-183">servicePrincipalNames</span><span class="sxs-lookup"><span data-stu-id="7a896-183">servicePrincipalNames</span></span>|<span data-ttu-id="7a896-184">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a896-184">String collection</span></span>|<span data-ttu-id="7a896-185">Contém a lista de **identificadoresUris**, copiados do [aplicativo](../resources/application.md) associado.</span><span class="sxs-lookup"><span data-stu-id="7a896-185">Contains the list of **identifiersUris**, copied over from the associated [application](../resources/application.md).</span></span> <span data-ttu-id="7a896-186">É possível adicionar valores adicionais aos aplicativos híbridos.</span><span class="sxs-lookup"><span data-stu-id="7a896-186">Additional values can be added to hybrid applications.</span></span> <span data-ttu-id="7a896-187">Esses valores podem ser usados ​​para identificar as permissões apresentadas por esse aplicativo no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7a896-187">These values can be used to identify the permissions exposed by this app within Azure AD.</span></span> <span data-ttu-id="7a896-188">Por exemplo,</span><span class="sxs-lookup"><span data-stu-id="7a896-188">For example,</span></span><ul><li><span data-ttu-id="7a896-189">Os aplicativos cliente solicitando permissões para este recurso podem usar esses URIs para especificar as permissões necessárias na propriedade **requiredResourceAccess** do manifesto do aplicativo, ou na lâmina "permissões de API" na experiência de registros de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="7a896-189">Client apps requesting permissions to this resource can use these URIs to specify needed permissions in the **requiredResourceAccess** property of their application manifest, or in the "API permissions" blade on the App registrations experience.</span></span></li><li><span data-ttu-id="7a896-190">Os aplicativos cliente podem especificar um URI de recurso com base nos valores dessa propriedade para adquirir um token de acesso, que é o URI retornado na declaração "aud".</span><span class="sxs-lookup"><span data-stu-id="7a896-190">Client apps can specify a resource URI which is based on the values of this property to acquire an access token, which is the URI returned in the “aud” claim.</span></span></li></ul><br><span data-ttu-id="7a896-p114">O operador é necessário para filtrar expressões nas propriedades multivalorizadas. Não pode ser anulado.</span><span class="sxs-lookup"><span data-stu-id="7a896-p114">The any operator is required for filter expressions on multi-valued properties. Not nullable.</span></span>|
|<span data-ttu-id="7a896-193">tags</span><span class="sxs-lookup"><span data-stu-id="7a896-193">tags</span></span>|<span data-ttu-id="7a896-194">Coleção String</span><span class="sxs-lookup"><span data-stu-id="7a896-194">String collection</span></span>| <span data-ttu-id="7a896-p115">Cadeias de caracteres personalizadas que podem ser usadas para categorizar e identificar o aplicativo. Não anulada.</span><span class="sxs-lookup"><span data-stu-id="7a896-p115">Custom strings that can be used to categorize and identify the application. Not nullable.</span></span> |
| <span data-ttu-id="7a896-197">tokenEncryptionKeyId</span><span class="sxs-lookup"><span data-stu-id="7a896-197">tokenEncryptionKeyId</span></span> |<span data-ttu-id="7a896-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a896-198">String</span></span>|<span data-ttu-id="7a896-199">Especifica a keyId de uma chave pública da coleção keyCredentials.</span><span class="sxs-lookup"><span data-stu-id="7a896-199">Specifies the keyId of a public key from the keyCredentials collection.</span></span> <span data-ttu-id="7a896-200">Quando configurado, o Azure AD emite tokens para este aplicativo criptografado usando a chave especificada por essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="7a896-200">When configured, Azure AD issues tokens for this application encrypted using the key specified by this property.</span></span> <span data-ttu-id="7a896-201">O código de aplicativo que recebe o token criptografado deve usar a chave privada correspondente para descriptografar o token a fim de que ele possa ser usado para o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="7a896-201">The application code that receives the encrypted token must use the matching private key to decrypt the token before it can be used for the signed-in user.</span></span>|

## <a name="response"></a><span data-ttu-id="7a896-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a896-202">Response</span></span>

<span data-ttu-id="7a896-203">Se bem-sucedido, este método retorna um código de resposta `204 No Content` e um objeto atualizado [servicePrincipal](../resources/serviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a896-203">If successful, this method returns a `204 No Content` response code and updated [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7a896-204">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7a896-204">Example</span></span>
### <a name="request"></a><span data-ttu-id="7a896-205">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a896-205">Request</span></span>
<span data-ttu-id="7a896-206">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7a896-206">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7a896-207">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a896-207">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_serviceprincipal"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/{id}
Content-type: application/json
Content-length: 391

{
  "appRoleAssignmentRequired": true
}
```
# <a name="c"></a>[<span data-ttu-id="7a896-208">C#</span><span class="sxs-lookup"><span data-stu-id="7a896-208">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7a896-209">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a896-209">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7a896-210">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a896-210">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7a896-211">Java</span><span class="sxs-lookup"><span data-stu-id="7a896-211">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7a896-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a896-212">Response</span></span>
<span data-ttu-id="7a896-p117">Aqui está um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="7a896-p117">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
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

