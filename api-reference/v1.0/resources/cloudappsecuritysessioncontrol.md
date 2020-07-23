---
title: tipo de recurso cloudAppSecuritySessionControl
description: Controle de sessão usado para impor verificações de segurança do aplicativo na nuvem.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6271ae47f94abb0c449dc6bd7a0930468d08d2b5
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384423"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a><span data-ttu-id="87eb8-103">tipo de recurso cloudAppSecuritySessionControl</span><span class="sxs-lookup"><span data-stu-id="87eb8-103">cloudAppSecuritySessionControl resource type</span></span>

<span data-ttu-id="87eb8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87eb8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="87eb8-105">Controle de sessão usado para impor verificações de segurança do aplicativo na nuvem.</span><span class="sxs-lookup"><span data-stu-id="87eb8-105">Session control used to enforce cloud app security checks.</span></span> <span data-ttu-id="87eb8-106">Inehrits do [controle de sessão de acesso condicional](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="87eb8-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="87eb8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="87eb8-107">Properties</span></span>

| <span data-ttu-id="87eb8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87eb8-108">Property</span></span>     | <span data-ttu-id="87eb8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="87eb8-109">Type</span></span>        | <span data-ttu-id="87eb8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="87eb8-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="87eb8-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="87eb8-111">isEnabled</span></span>     |<span data-ttu-id="87eb8-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="87eb8-112">Boolean</span></span>      | <span data-ttu-id="87eb8-113">Especifica se o controle de sessão está habilitado.</span><span class="sxs-lookup"><span data-stu-id="87eb8-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="87eb8-114">cloudAppSecurityType</span><span class="sxs-lookup"><span data-stu-id="87eb8-114">cloudAppSecurityType</span></span>|<span data-ttu-id="87eb8-115">String</span><span class="sxs-lookup"><span data-stu-id="87eb8-115">String</span></span>| <span data-ttu-id="87eb8-116">Os valores possíveis são: `mcasConfigured`, `monitorOnly`, `blockDownloads`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="87eb8-116">Possible values are: `mcasConfigured`, `monitorOnly`, `blockDownloads`, `unknownFutureValue`.</span></span> <span data-ttu-id="87eb8-117">Para obter mais informações, consulte [Deploy Conditional Access app Control for refeatured apps](https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad).</span><span class="sxs-lookup"><span data-stu-id="87eb8-117">For more information, see [Deploy Conditional Access App Control for featured apps](https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad).</span></span> |

## <a name="relationships"></a><span data-ttu-id="87eb8-118">Relações</span><span class="sxs-lookup"><span data-stu-id="87eb8-118">Relationships</span></span>

<span data-ttu-id="87eb8-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="87eb8-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="87eb8-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="87eb8-120">JSON representation</span></span>

<span data-ttu-id="87eb8-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="87eb8-121">The following is a JSON representation of the resource.</span></span>

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
