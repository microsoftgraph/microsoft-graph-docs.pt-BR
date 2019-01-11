---
title: tipo de recurso de agreementFileData
description: Representa o blob do Azure Active Directory termos (Azure AD) do arquivo do contrato de uso.
localization_priority: Normal
ms.openlocfilehash: 64de3a72ad648225f24429987f5729f76ed8a2e7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815212"
---
# <a name="agreementfiledata-resource-type"></a><span data-ttu-id="103a0-103">tipo de recurso de agreementFileData</span><span class="sxs-lookup"><span data-stu-id="103a0-103">agreementFileData resource type</span></span>

> <span data-ttu-id="103a0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="103a0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="103a0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="103a0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="103a0-106">Representa o blob do Azure Active Directory termos (Azure AD) do arquivo do contrato de uso.</span><span class="sxs-lookup"><span data-stu-id="103a0-106">Represents the blob of an Azure Active Directory (Azure AD) terms of use agreement file.</span></span>

## <a name="properties"></a><span data-ttu-id="103a0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="103a0-107">Properties</span></span>
| <span data-ttu-id="103a0-108">Método</span><span class="sxs-lookup"><span data-stu-id="103a0-108">Method</span></span>       | <span data-ttu-id="103a0-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="103a0-109">Return Type</span></span> | <span data-ttu-id="103a0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="103a0-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="103a0-111">data</span><span class="sxs-lookup"><span data-stu-id="103a0-111">data</span></span>|<span data-ttu-id="103a0-112">Binária</span><span class="sxs-lookup"><span data-stu-id="103a0-112">Binary</span></span>|<span data-ttu-id="103a0-113">Dados que representam as condições de usar o documento PDF.</span><span class="sxs-lookup"><span data-stu-id="103a0-113">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="103a0-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="103a0-114">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="103a0-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="103a0-115">JSON representation</span></span>

<span data-ttu-id="103a0-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="103a0-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFileData"
}-->

```json
{
  "data": "Binary"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "agreementFileData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
