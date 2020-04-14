---
title: tipo de recurso apiApplication
description: Especifica as configurações para um aplicativo da API Web.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: bad5b54e85a97c209b2b6e65c5555b4c97fe6de8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43408236"
---
# <a name="apiapplication-resource-type"></a><span data-ttu-id="e00c2-103">tipo de recurso apiApplication</span><span class="sxs-lookup"><span data-stu-id="e00c2-103">apiApplication resource type</span></span>

<span data-ttu-id="e00c2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e00c2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e00c2-105">Especifica configurações para um aplicativo que implementa uma API Web.</span><span class="sxs-lookup"><span data-stu-id="e00c2-105">Specifies settings for an application that implements a web API.</span></span>

## <a name="properties"></a><span data-ttu-id="e00c2-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e00c2-106">Properties</span></span>

| <span data-ttu-id="e00c2-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e00c2-107">Property</span></span> | <span data-ttu-id="e00c2-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e00c2-108">Type</span></span> | <span data-ttu-id="e00c2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e00c2-109">Description</span></span> |
|:---------------|:--------|:----------|
|`acceptMappedClaims`| <span data-ttu-id="e00c2-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="e00c2-110">Boolean</span></span> | <span data-ttu-id="e00c2-111">Quando true, permite que um aplicativo use o mapeamento de declarações sem especificar uma chave de assinatura personalizada.</span><span class="sxs-lookup"><span data-stu-id="e00c2-111">When true, allows an application to use claims mapping without specifying a custom signing key.</span></span> |
|`knownClientApplications`| <span data-ttu-id="e00c2-112">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="e00c2-112">Guid collection</span></span> |<span data-ttu-id="e00c2-113">Usado para o consentimento de agrupamento se você tiver uma solução que contenha duas partes: um aplicativo cliente e um aplicativo de API Web personalizado.</span><span class="sxs-lookup"><span data-stu-id="e00c2-113">Used for bundling consent if you have a solution that contains two parts: a client app and a custom web API app.</span></span> <span data-ttu-id="e00c2-114">Se você definir a appID do aplicativo cliente com esse valor, o usuário só consenti uma vez para o aplicativo cliente.</span><span class="sxs-lookup"><span data-stu-id="e00c2-114">If you set the appID of the client app to this value, the user only consents once to the client app.</span></span> <span data-ttu-id="e00c2-115">O Azure AD sabe que a reenvio para o cliente significa implicitamente Confira a API Web e automaticamente provisiona entidades de serviço para ambas as APIs ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="e00c2-115">Azure AD knows that consenting to the client means implicitly consenting to the web API and automatically provisions service principals for both APIs at the same time.</span></span> <span data-ttu-id="e00c2-116">O cliente e o aplicativo da API Web devem ser registrados no mesmo locatário.</span><span class="sxs-lookup"><span data-stu-id="e00c2-116">Both the client and the web API app must be registered in the same tenant.</span></span>|
|`oauth2PermissionScopes`| <span data-ttu-id="e00c2-117">coleção [permissionScope](permissionscope.md)</span><span class="sxs-lookup"><span data-stu-id="e00c2-117">[permissionScope](permissionscope.md) collection</span></span> | <span data-ttu-id="e00c2-118">A coleção de escopos de permissão OAuth 2,0 que o aplicativo Web API (recurso) expõe para aplicativos cliente.</span><span class="sxs-lookup"><span data-stu-id="e00c2-118">The collection of OAuth 2.0 permission scopes that the web API (resource) application exposes to client applications.</span></span> <span data-ttu-id="e00c2-119">Esses escopos de permissão podem ser concedidos aos aplicativos cliente durante o consentimento.</span><span class="sxs-lookup"><span data-stu-id="e00c2-119">These permission scopes may be granted to client applications during consent.</span></span> |
|`preAuthorizedApplications`| <span data-ttu-id="e00c2-120">coleção [preauthorizedapplication e](preauthorizedapplication.md)</span><span class="sxs-lookup"><span data-stu-id="e00c2-120">[preAuthorizedApplication](preauthorizedapplication.md) collection</span></span> | <span data-ttu-id="e00c2-121">Lista os aplicativos cliente que são previamente autorizados com as permissões delegadas especificadas para acessar as APIs desse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e00c2-121">Lists the client applications that are pre-authorized with the specified delegated permissions to access this application's APIs.</span></span> <span data-ttu-id="e00c2-122">Os usuários não precisam ser consentidos em qualquer aplicativo pré autorizado (para as permissões especificadas).</span><span class="sxs-lookup"><span data-stu-id="e00c2-122">Users are not required to consent to any pre-authorized application (for the permissions specified).</span></span> <span data-ttu-id="e00c2-123">No entanto, qualquer permissão adicional que não esteja listada no preAuthorizedApplications (solicitado por meio de consentimento incremental, por exemplo) exigirá o consentimento do usuário.</span><span class="sxs-lookup"><span data-stu-id="e00c2-123">However, any additional permissions not listed in preAuthorizedApplications (requested through incremental consent for example) will require user consent.</span></span> |
|`requestedAccessTokenVersion`| <span data-ttu-id="e00c2-124">Int32</span><span class="sxs-lookup"><span data-stu-id="e00c2-124">Int32</span></span> | <span data-ttu-id="e00c2-125">Especifica a versão do token de acesso esperada por este recurso.</span><span class="sxs-lookup"><span data-stu-id="e00c2-125">Specifies the access token version expected by this resource.</span></span> <span data-ttu-id="e00c2-126">Isso altera a versão e o formato do JWT produzido independentemente do ponto de extremidade ou cliente usado para solicitar o token de acesso.</span><span class="sxs-lookup"><span data-stu-id="e00c2-126">This changes the version and format of the JWT produced independent of the endpoint or client used to request the access token.</span></span> <br><br> <span data-ttu-id="e00c2-127">O ponto de extremidade usado, v 1.0 ou v 2.0, é escolhido pelo cliente e só impacta a versão do id_tokens.</span><span class="sxs-lookup"><span data-stu-id="e00c2-127">The endpoint used, v1.0 or v2.0, is chosen by the client and only impacts the version of id_tokens.</span></span> <span data-ttu-id="e00c2-128">Os recursos precisam ser configurados `requestedAccessTokenVersion` explicitamente para indicar o formato do token de acesso suportado.</span><span class="sxs-lookup"><span data-stu-id="e00c2-128">Resources need to explicitly configure `requestedAccessTokenVersion` to indicate the supported access token format.</span></span> <br><br> <span data-ttu-id="e00c2-129">Os valores possíveis `requestedAccessTokenVersion` para `1`são `2`,, `null`ou.</span><span class="sxs-lookup"><span data-stu-id="e00c2-129">Possible values for `requestedAccessTokenVersion` are `1`, `2`, or `null`.</span></span> <span data-ttu-id="e00c2-130">Se o valor for `null`, este padrão será `1`, que corresponde ao ponto de extremidade v 1.0.</span><span class="sxs-lookup"><span data-stu-id="e00c2-130">If the value is `null`, this defaults to `1`, which corresponds to the v1.0 endpoint.</span></span> <br><br> <span data-ttu-id="e00c2-131">Se `signInAudience` no aplicativo estiver configurado como `AzureADandPersonalMicrosoftAccount`, o valor dessa propriedade deverá ser`2`</span><span class="sxs-lookup"><span data-stu-id="e00c2-131">If `signInAudience` on the application is configured as `AzureADandPersonalMicrosoftAccount`, the value for this property must be `2`</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e00c2-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e00c2-132">JSON representation</span></span>
<span data-ttu-id="e00c2-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e00c2-133">Here is a JSON representation of the resource.</span></span>

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
