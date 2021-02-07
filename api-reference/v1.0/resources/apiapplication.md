---
title: Tipo de recurso apiApplication
description: Especifica configurações para um aplicativo de API Web.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 81d0431a21ca230d96de0dd8f826a166fa16bace
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134999"
---
# <a name="apiapplication-resource-type"></a><span data-ttu-id="68476-103">Tipo de recurso apiApplication</span><span class="sxs-lookup"><span data-stu-id="68476-103">apiApplication resource type</span></span>

<span data-ttu-id="68476-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68476-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="68476-105">Especifica configurações para um aplicativo que implementa uma API Web.</span><span class="sxs-lookup"><span data-stu-id="68476-105">Specifies settings for an application that implements a web API.</span></span>

## <a name="properties"></a><span data-ttu-id="68476-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="68476-106">Properties</span></span>

| <span data-ttu-id="68476-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68476-107">Property</span></span> | <span data-ttu-id="68476-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="68476-108">Type</span></span> | <span data-ttu-id="68476-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="68476-109">Description</span></span> |
|:---------------|:--------|:----------|
|`acceptMappedClaims`| <span data-ttu-id="68476-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="68476-110">Boolean</span></span> | <span data-ttu-id="68476-111">Quando verdadeiro, permite que um aplicativo use o mapeamento de declarações sem especificar uma chave de assinatura personalizada.</span><span class="sxs-lookup"><span data-stu-id="68476-111">When true, allows an application to use claims mapping without specifying a custom signing key.</span></span> |
|`knownClientApplications`| <span data-ttu-id="68476-112">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="68476-112">Guid collection</span></span> |<span data-ttu-id="68476-113">Usado para o consentimento de ad bundling se você tiver uma solução que contenha duas partes: um aplicativo cliente e um aplicativo de API Web personalizado.</span><span class="sxs-lookup"><span data-stu-id="68476-113">Used for bundling consent if you have a solution that contains two parts: a client app and a custom web API app.</span></span> <span data-ttu-id="68476-114">Se você definir a appID do aplicativo cliente com esse valor, o usuário só consente uma vez com o aplicativo cliente.</span><span class="sxs-lookup"><span data-stu-id="68476-114">If you set the appID of the client app to this value, the user only consents once to the client app.</span></span> <span data-ttu-id="68476-115">O Azure AD sabe que consentir com o cliente significa consentir implicitamente com a API da Web e provisionar automaticamente entidades de serviço para ambas as APIs ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="68476-115">Azure AD knows that consenting to the client means implicitly consenting to the web API and automatically provisions service principals for both APIs at the same time.</span></span> <span data-ttu-id="68476-116">O cliente e o aplicativo da API Web devem ser registrados no mesmo locatário.</span><span class="sxs-lookup"><span data-stu-id="68476-116">Both the client and the web API app must be registered in the same tenant.</span></span>|
|`oauth2PermissionScopes`| <span data-ttu-id="68476-117">coleção [permissionScope](permissionscope.md)</span><span class="sxs-lookup"><span data-stu-id="68476-117">[permissionScope](permissionscope.md) collection</span></span> | <span data-ttu-id="68476-118">A definição das permissões delegadas expostas pela API Web representada por esse registro de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="68476-118">The definition of the delegated permissions exposed by the web API represented by this application registration.</span></span> <span data-ttu-id="68476-119">Essas permissões delegadas podem ser solicitadas por um aplicativo cliente e podem ser concedidas por usuários ou administradores durante o consentimento.</span><span class="sxs-lookup"><span data-stu-id="68476-119">These delegated permissions may be requested by a client application, and may be granted by users or administrators during consent.</span></span> <span data-ttu-id="68476-120">As permissões delegadas às vezes são conhecidas como escopos OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="68476-120">Delegated permissions are sometimes referred to as OAuth 2.0 scopes.</span></span> |
|`preAuthorizedApplications`| <span data-ttu-id="68476-121">[Coleção preAuthorizedApplication](preauthorizedapplication.md)</span><span class="sxs-lookup"><span data-stu-id="68476-121">[preAuthorizedApplication](preauthorizedapplication.md) collection</span></span> | <span data-ttu-id="68476-122">Lista os aplicativos cliente que são pré-autorizados com as permissões delegadas especificadas para acessar as APIs desse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="68476-122">Lists the client applications that are pre-authorized with the specified delegated permissions to access this application's APIs.</span></span> <span data-ttu-id="68476-123">Os usuários não precisam consentir com qualquer aplicativo pré-autorizado (para as permissões especificadas).</span><span class="sxs-lookup"><span data-stu-id="68476-123">Users are not required to consent to any pre-authorized application (for the permissions specified).</span></span> <span data-ttu-id="68476-124">No entanto, quaisquer permissões adicionais não listadas em preAuthorizedApplications (solicitadas por meio de consentimento incremental, por exemplo) exigirão o consentimento do usuário.</span><span class="sxs-lookup"><span data-stu-id="68476-124">However, any additional permissions not listed in preAuthorizedApplications (requested through incremental consent for example) will require user consent.</span></span> |
|`requestedAccessTokenVersion`| <span data-ttu-id="68476-125">Int32</span><span class="sxs-lookup"><span data-stu-id="68476-125">Int32</span></span> | <span data-ttu-id="68476-126">Especifica a versão do token de acesso esperada por esse recurso.</span><span class="sxs-lookup"><span data-stu-id="68476-126">Specifies the access token version expected by this resource.</span></span> <span data-ttu-id="68476-127">Isso altera a versão e o formato do JWT produzido independentemente do ponto de extremidade ou do cliente usado para solicitar o token de acesso.</span><span class="sxs-lookup"><span data-stu-id="68476-127">This changes the version and format of the JWT produced independent of the endpoint or client used to request the access token.</span></span> <br><br> <span data-ttu-id="68476-128">O ponto de extremidade usado, v1.0 ou v2.0, é escolhido pelo cliente e afeta apenas a versão do id_tokens.</span><span class="sxs-lookup"><span data-stu-id="68476-128">The endpoint used, v1.0 or v2.0, is chosen by the client and only impacts the version of id_tokens.</span></span> <span data-ttu-id="68476-129">Os recursos precisam ser explicitamente `requestedAccessTokenVersion` configuradas para indicar o formato de token de acesso com suporte.</span><span class="sxs-lookup"><span data-stu-id="68476-129">Resources need to explicitly configure `requestedAccessTokenVersion` to indicate the supported access token format.</span></span> <br><br> <span data-ttu-id="68476-130">Os valores `requestedAccessTokenVersion` possíveis para `1` são , `2` ou `null` .</span><span class="sxs-lookup"><span data-stu-id="68476-130">Possible values for `requestedAccessTokenVersion` are `1`, `2`, or `null`.</span></span> <span data-ttu-id="68476-131">Se o valor for , o padrão é , que corresponde ao ponto de `null` `1` extremidade v1.0.</span><span class="sxs-lookup"><span data-stu-id="68476-131">If the value is `null`, this defaults to `1`, which corresponds to the v1.0 endpoint.</span></span> <br><br> <span data-ttu-id="68476-132">Se `signInAudience` no aplicativo estiver configurado como , o valor dessa propriedade deverá `AzureADandPersonalMicrosoftAccount` ser `2`</span><span class="sxs-lookup"><span data-stu-id="68476-132">If `signInAudience` on the application is configured as `AzureADandPersonalMicrosoftAccount`, the value for this property must be `2`</span></span> |

## <a name="json-representation"></a><span data-ttu-id="68476-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="68476-133">JSON representation</span></span>

<span data-ttu-id="68476-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="68476-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.apiApplication"
}-->

```json
{
  "acceptMappedClaims": true,
  "knownClientApplications": ["Guid"],
  "oauth2PermissionScopes": [{"@odata.type": "microsoft.graph.permissionScope"}],
  "preAuthorizedApplications": [{"@odata.type": "microsoft.graph.preAuthorizedApplication"}],
  "requestedAccessTokenVersion": 2
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "api resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

