---
title: tipo de recurso de erro genérico
description: Um erro de finalidade geral.
localization_priority: Normal
ms.openlocfilehash: 744266ef8ffb17c4af4168d6239e5a5a30561936
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823566"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="c097e-103">tipo de recurso de erro genérico</span><span class="sxs-lookup"><span data-stu-id="c097e-103">genericError resource type</span></span>

> <span data-ttu-id="c097e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c097e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c097e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c097e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c097e-106">Um erro de finalidade geral.</span><span class="sxs-lookup"><span data-stu-id="c097e-106">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="c097e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c097e-107">Properties</span></span>

| <span data-ttu-id="c097e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c097e-108">Property</span></span> | <span data-ttu-id="c097e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c097e-109">Type</span></span> | <span data-ttu-id="c097e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c097e-110">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="c097e-111">mensagem</span><span class="sxs-lookup"><span data-stu-id="c097e-111">message</span></span> | <span data-ttu-id="c097e-112">String</span><span class="sxs-lookup"><span data-stu-id="c097e-112">String</span></span> | <span data-ttu-id="c097e-113">A mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="c097e-113">The error message.</span></span> |
| <span data-ttu-id="c097e-114">código</span><span class="sxs-lookup"><span data-stu-id="c097e-114">code</span></span> | <span data-ttu-id="c097e-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c097e-115">String</span></span> | <span data-ttu-id="c097e-116">O código do erro.</span><span class="sxs-lookup"><span data-stu-id="c097e-116">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c097e-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c097e-117">JSON representation</span></span>

<span data-ttu-id="c097e-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c097e-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.genericError"
}-->

```json
{
  "message": "String",
  "code": "String"
}
```
