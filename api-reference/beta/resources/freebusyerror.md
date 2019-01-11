---
title: tipo de recurso de freeBusyError
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: 63cfc4b14ba6176d582155df57b7f7f787e63cf4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889765"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="397b1-104">tipo de recurso de freeBusyError</span><span class="sxs-lookup"><span data-stu-id="397b1-104">freeBusyError resource type</span></span>

 > <span data-ttu-id="397b1-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="397b1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="397b1-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="397b1-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="397b1-107">Representa informações de erro de tentar obter a disponibilidade de um usuário, uma lista de distribuição ou um recurso.</span><span class="sxs-lookup"><span data-stu-id="397b1-107">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="397b1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="397b1-108">Properties</span></span>
| <span data-ttu-id="397b1-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="397b1-109">Property</span></span>     | <span data-ttu-id="397b1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="397b1-110">Type</span></span>   |<span data-ttu-id="397b1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="397b1-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="397b1-112">mensagem</span><span class="sxs-lookup"><span data-stu-id="397b1-112">message</span></span> |<span data-ttu-id="397b1-113">String</span><span class="sxs-lookup"><span data-stu-id="397b1-113">String</span></span> |<span data-ttu-id="397b1-114">Descreve o erro.</span><span class="sxs-lookup"><span data-stu-id="397b1-114">Describes the error.</span></span> |
|<span data-ttu-id="397b1-115">responseCode</span><span class="sxs-lookup"><span data-stu-id="397b1-115">responseCode</span></span> |<span data-ttu-id="397b1-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="397b1-116">String</span></span> |<span data-ttu-id="397b1-117">O código de resposta do consultando para a disponibilidade do usuário, lista de distribuição ou recurso.</span><span class="sxs-lookup"><span data-stu-id="397b1-117">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="397b1-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="397b1-118">JSON representation</span></span>

<span data-ttu-id="397b1-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="397b1-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.freeBusyError"
}-->

```json
{
  "message": "String",
  "responseCode": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "freeBusyError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
