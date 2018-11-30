---
title: tipo de recurso de erro genérico
description: Um erro de finalidade geral.
ms.openlocfilehash: caf3fbb99ad521fd807138ab230f6a1b8ae7bb16
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033830"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="3dc1c-103">tipo de recurso de erro genérico</span><span class="sxs-lookup"><span data-stu-id="3dc1c-103">genericError resource type</span></span>

> <span data-ttu-id="3dc1c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3dc1c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3dc1c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3dc1c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3dc1c-106">Um erro de finalidade geral.</span><span class="sxs-lookup"><span data-stu-id="3dc1c-106">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="3dc1c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3dc1c-107">Properties</span></span>

| <span data-ttu-id="3dc1c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3dc1c-108">Property</span></span> | <span data-ttu-id="3dc1c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3dc1c-109">Type</span></span> | <span data-ttu-id="3dc1c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3dc1c-110">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="3dc1c-111">mensagem</span><span class="sxs-lookup"><span data-stu-id="3dc1c-111">message</span></span> | <span data-ttu-id="3dc1c-112">String</span><span class="sxs-lookup"><span data-stu-id="3dc1c-112">String</span></span> | <span data-ttu-id="3dc1c-113">A mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="3dc1c-113">The error message.</span></span> |
| <span data-ttu-id="3dc1c-114">código</span><span class="sxs-lookup"><span data-stu-id="3dc1c-114">code</span></span> | <span data-ttu-id="3dc1c-115">String</span><span class="sxs-lookup"><span data-stu-id="3dc1c-115">String</span></span> | <span data-ttu-id="3dc1c-116">O código do erro.</span><span class="sxs-lookup"><span data-stu-id="3dc1c-116">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3dc1c-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3dc1c-117">JSON representation</span></span>

<span data-ttu-id="3dc1c-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3dc1c-118">Here is a JSON representation of the resource.</span></span>

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