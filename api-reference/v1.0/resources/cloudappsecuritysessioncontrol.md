---
title: Tipo de recurso cloudAppSecuritySessionControl
description: Controle de sessão usado para impor verificações de segurança do aplicativo na nuvem.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c52322928b5ef2e2538031ae8c251bc9c1a4caac
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962508"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a><span data-ttu-id="749b2-103">Tipo de recurso cloudAppSecuritySessionControl</span><span class="sxs-lookup"><span data-stu-id="749b2-103">cloudAppSecuritySessionControl resource type</span></span>

<span data-ttu-id="749b2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="749b2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="749b2-105">Controle de sessão usado para impor verificações de segurança do aplicativo na nuvem.</span><span class="sxs-lookup"><span data-stu-id="749b2-105">Session control used to enforce cloud app security checks.</span></span> <span data-ttu-id="749b2-106">Inehrits do Controle de Sessão [de Acesso Condicional](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="749b2-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="749b2-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="749b2-107">Properties</span></span>

| <span data-ttu-id="749b2-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="749b2-108">Property</span></span>     | <span data-ttu-id="749b2-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="749b2-109">Type</span></span>        | <span data-ttu-id="749b2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="749b2-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="749b2-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="749b2-111">isEnabled</span></span>     |<span data-ttu-id="749b2-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="749b2-112">Boolean</span></span>      | <span data-ttu-id="749b2-113">Especifica se o controle de sessão está habilitado.</span><span class="sxs-lookup"><span data-stu-id="749b2-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="749b2-114">cloudAppSecurityType</span><span class="sxs-lookup"><span data-stu-id="749b2-114">cloudAppSecurityType</span></span>|<span data-ttu-id="749b2-115">cloudAppSecuritySessionControlType</span><span class="sxs-lookup"><span data-stu-id="749b2-115">cloudAppSecuritySessionControlType</span></span>| <span data-ttu-id="749b2-116">Os valores possíveis são: `mcasConfigured`, `monitorOnly`, `blockDownloads`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="749b2-116">Possible values are: `mcasConfigured`, `monitorOnly`, `blockDownloads`, `unknownFutureValue`.</span></span> <span data-ttu-id="749b2-117">Para obter mais informações, [consulte Deploy Conditional Access App Control for featured apps](/cloud-app-security/proxy-deployment-aad).</span><span class="sxs-lookup"><span data-stu-id="749b2-117">For more information, see [Deploy Conditional Access App Control for featured apps](/cloud-app-security/proxy-deployment-aad).</span></span> |

## <a name="relationships"></a><span data-ttu-id="749b2-118">Relações</span><span class="sxs-lookup"><span data-stu-id="749b2-118">Relationships</span></span>

<span data-ttu-id="749b2-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="749b2-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="749b2-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="749b2-120">JSON representation</span></span>

<span data-ttu-id="749b2-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="749b2-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cloudAppSecuritySessionControl",
  "baseType": "microsoft.graph.conditionalAccessSessionControl"
}-->

```json
{
  "isEnabled": true,
  "cloudAppSecurityType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "cloudAppSecuritySessionControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
