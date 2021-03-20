---
title: Tipo de recurso apiApplication
description: Especifica configurações para um aplicativo de API Web.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 1a01418fad74d48a1697bace91833d880a94f467
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955963"
---
# <a name="apiapplication-resource-type"></a><span data-ttu-id="e3596-103">Tipo de recurso apiApplication</span><span class="sxs-lookup"><span data-stu-id="e3596-103">apiApplication resource type</span></span>

<span data-ttu-id="e3596-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3596-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e3596-105">Especifica configurações para um aplicativo que implementa uma API Web.</span><span class="sxs-lookup"><span data-stu-id="e3596-105">Specifies settings for an application that implements a web API.</span></span>

## <a name="properties"></a><span data-ttu-id="e3596-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e3596-106">Properties</span></span>

| <span data-ttu-id="e3596-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3596-107">Property</span></span> | <span data-ttu-id="e3596-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3596-108">Type</span></span> | <span data-ttu-id="e3596-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3596-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e3596-110">acceptMappedClaims</span><span class="sxs-lookup"><span data-stu-id="e3596-110">acceptMappedClaims</span></span>| <span data-ttu-id="e3596-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="e3596-111">Boolean</span></span> | <span data-ttu-id="e3596-112">Quando `true` , permite que um aplicativo use o mapeamento de declarações sem especificar uma chave de assinatura personalizada.</span><span class="sxs-lookup"><span data-stu-id="e3596-112">When `true`, allows an application to use claims mapping without specifying a custom signing key.</span></span> |
|<span data-ttu-id="e3596-113">knownClientApplications</span><span class="sxs-lookup"><span data-stu-id="e3596-113">knownClientApplications</span></span>| <span data-ttu-id="e3596-114">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="e3596-114">Guid collection</span></span> |<span data-ttu-id="e3596-115">Usado para o consentimento em comum se você tiver uma solução que contenha duas partes: um aplicativo cliente e um aplicativo de API Web personalizado.</span><span class="sxs-lookup"><span data-stu-id="e3596-115">Used for bundling consent if you have a solution that contains two parts: a client app and a custom web API app.</span></span> <span data-ttu-id="e3596-116">Se você definir a appID do aplicativo cliente para esse valor, o usuário só consente uma vez no aplicativo cliente.</span><span class="sxs-lookup"><span data-stu-id="e3596-116">If you set the appID of the client app to this value, the user only consents once to the client app.</span></span> <span data-ttu-id="e3596-117">O Azure AD sabe que consentir com o cliente significa consentir implicitamente a API da Web e provisionar automaticamente as entidades de serviço para ambas as APIs ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="e3596-117">Azure AD knows that consenting to the client means implicitly consenting to the web API and automatically provisions service principals for both APIs at the same time.</span></span> <span data-ttu-id="e3596-118">Tanto o cliente quanto o aplicativo api web devem ser registrados no mesmo locatário.</span><span class="sxs-lookup"><span data-stu-id="e3596-118">Both the client and the web API app must be registered in the same tenant.</span></span>|
|<span data-ttu-id="e3596-119">oauth2PermissionScopes</span><span class="sxs-lookup"><span data-stu-id="e3596-119">oauth2PermissionScopes</span></span>| <span data-ttu-id="e3596-120">coleção [permissionScope](permissionscope.md)</span><span class="sxs-lookup"><span data-stu-id="e3596-120">[permissionScope](permissionscope.md) collection</span></span> | <span data-ttu-id="e3596-121">A definição das permissões delegadas expostas pela API web representada pelo registro desse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e3596-121">The definition of the delegated permissions exposed by the web API represented by this application registration.</span></span> <span data-ttu-id="e3596-122">Essas permissões delegadas podem ser solicitadas por um aplicativo cliente e podem ser concedidas por usuários ou administradores durante o consentimento.</span><span class="sxs-lookup"><span data-stu-id="e3596-122">These delegated permissions may be requested by a client application, and may be granted by users or administrators during consent.</span></span> <span data-ttu-id="e3596-123">As permissões delegadas às vezes são conhecidas como escopos OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="e3596-123">Delegated permissions are sometimes referred to as OAuth 2.0 scopes.</span></span> |
|<span data-ttu-id="e3596-124">preAuthorizedApplications</span><span class="sxs-lookup"><span data-stu-id="e3596-124">preAuthorizedApplications</span></span>| <span data-ttu-id="e3596-125">[coleção preAuthorizedApplication](preauthorizedapplication.md)</span><span class="sxs-lookup"><span data-stu-id="e3596-125">[preAuthorizedApplication](preauthorizedapplication.md) collection</span></span> | <span data-ttu-id="e3596-126">Lista os aplicativos cliente pré-autorizados com as permissões delegadas especificadas para acessar as APIs desse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e3596-126">Lists the client applications that are pre-authorized with the specified delegated permissions to access this application's APIs.</span></span> <span data-ttu-id="e3596-127">Os usuários não precisam consentir com nenhum aplicativo pré-autorizado (para as permissões especificadas).</span><span class="sxs-lookup"><span data-stu-id="e3596-127">Users are not required to consent to any pre-authorized application (for the permissions specified).</span></span> <span data-ttu-id="e3596-128">No entanto, quaisquer permissões adicionais não listadas em preAuthorizedApplications (solicitadas por meio do consentimento incremental, por exemplo) exigirão o consentimento do usuário.</span><span class="sxs-lookup"><span data-stu-id="e3596-128">However, any additional permissions not listed in preAuthorizedApplications (requested through incremental consent for example) will require user consent.</span></span> |
|<span data-ttu-id="e3596-129">requestedAccessTokenVersion</span><span class="sxs-lookup"><span data-stu-id="e3596-129">requestedAccessTokenVersion</span></span>| <span data-ttu-id="e3596-130">Int32</span><span class="sxs-lookup"><span data-stu-id="e3596-130">Int32</span></span> | <span data-ttu-id="e3596-131">Especifica a versão do token de acesso esperada por esse recurso.</span><span class="sxs-lookup"><span data-stu-id="e3596-131">Specifies the access token version expected by this resource.</span></span> <span data-ttu-id="e3596-132">Isso altera a versão e o formato do JWT produzido independentemente do ponto de extremidade ou cliente usado para solicitar o token de acesso.</span><span class="sxs-lookup"><span data-stu-id="e3596-132">This changes the version and format of the JWT produced independent of the endpoint or client used to request the access token.</span></span> <br><br> <span data-ttu-id="e3596-133">O ponto de extremidade usado, v1.0 ou v2.0, é escolhido pelo cliente e afeta apenas a versão do id_tokens.</span><span class="sxs-lookup"><span data-stu-id="e3596-133">The endpoint used, v1.0 or v2.0, is chosen by the client and only impacts the version of id_tokens.</span></span> <span data-ttu-id="e3596-134">Os recursos precisam configurar explicitamente **requestedAccessTokenVersion** para indicar o formato de token de acesso suportado.</span><span class="sxs-lookup"><span data-stu-id="e3596-134">Resources need to explicitly configure **requestedAccessTokenVersion** to indicate the supported access token format.</span></span> <br><br> <span data-ttu-id="e3596-135">Os valores possíveis **para requestedAccessTokenVersion** `1` são , ou `2` `null` .</span><span class="sxs-lookup"><span data-stu-id="e3596-135">Possible values for **requestedAccessTokenVersion** are `1`, `2`, or `null`.</span></span> <span data-ttu-id="e3596-136">Se o valor for , isso padrão será , que corresponde ao ponto `null` `1` de extremidade v1.0.</span><span class="sxs-lookup"><span data-stu-id="e3596-136">If the value is `null`, this defaults to `1`, which corresponds to the v1.0 endpoint.</span></span> <br><br> <span data-ttu-id="e3596-137">Se **signInAudience** no aplicativo estiver configurado como `AzureADandPersonalMicrosoftAccount` , o valor dessa propriedade deve ser `2`</span><span class="sxs-lookup"><span data-stu-id="e3596-137">If **signInAudience** on the application is configured as `AzureADandPersonalMicrosoftAccount`, the value for this property must be `2`</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e3596-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e3596-138">JSON representation</span></span>

<span data-ttu-id="e3596-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e3596-139">Here is a JSON representation of the resource.</span></span>

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

