---
title: Tipo de recurso cloudAppSecuritySessionControl
description: Controle de sessão usado para impor verificações de segurança do aplicativo na nuvem.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 630c558981b3dc9bbb0ec48c9a81ff74868c43bb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941827"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a><span data-ttu-id="84687-103">Tipo de recurso cloudAppSecuritySessionControl</span><span class="sxs-lookup"><span data-stu-id="84687-103">cloudAppSecuritySessionControl resource type</span></span>

<span data-ttu-id="84687-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84687-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84687-105">Controle de sessão usado para impor verificações de segurança do aplicativo na nuvem.</span><span class="sxs-lookup"><span data-stu-id="84687-105">Session control used to enforce cloud app security checks.</span></span> <span data-ttu-id="84687-106">Inehrits do Controle de Sessão [de Acesso Condicional](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="84687-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="84687-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="84687-107">Properties</span></span>

| <span data-ttu-id="84687-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84687-108">Property</span></span>     | <span data-ttu-id="84687-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="84687-109">Type</span></span>        | <span data-ttu-id="84687-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="84687-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="84687-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="84687-111">isEnabled</span></span>     |<span data-ttu-id="84687-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="84687-112">Boolean</span></span>      | <span data-ttu-id="84687-113">Especifica se o controle de sessão está habilitado.</span><span class="sxs-lookup"><span data-stu-id="84687-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="84687-114">cloudAppSecurityType</span><span class="sxs-lookup"><span data-stu-id="84687-114">cloudAppSecurityType</span></span>|<span data-ttu-id="84687-115">cloudAppSecuritySessionControlType</span><span class="sxs-lookup"><span data-stu-id="84687-115">cloudAppSecuritySessionControlType</span></span>| <span data-ttu-id="84687-116">Os valores possíveis são: `mcasConfigured`, `monitorOnly`, `blockDownloads`.</span><span class="sxs-lookup"><span data-stu-id="84687-116">Possible values are: `mcasConfigured`, `monitorOnly`, `blockDownloads`.</span></span> <span data-ttu-id="84687-117">Saiba mais sobre esses valores aqui: https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad#step-1-create-an-azure-ad-conditional-access-test-policy-</span><span class="sxs-lookup"><span data-stu-id="84687-117">Learn more about these values here: https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad#step-1-create-an-azure-ad-conditional-access-test-policy-</span></span> |

## <a name="relationships"></a><span data-ttu-id="84687-118">Relações</span><span class="sxs-lookup"><span data-stu-id="84687-118">Relationships</span></span>

<span data-ttu-id="84687-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="84687-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="84687-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="84687-120">JSON representation</span></span>

<span data-ttu-id="84687-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="84687-121">The following is a JSON representation of the resource.</span></span>

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

