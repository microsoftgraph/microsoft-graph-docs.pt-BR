---
title: Tipo de recurso mimeContent
description: Contém as propriedades de um conteúdo genérico MIME.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 62132b9e55b8130f82fc8414cbb6e90ba34bb70f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413455"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="9975f-103">Tipo de recurso mimeContent</span><span class="sxs-lookup"><span data-stu-id="9975f-103">mimeContent resource type</span></span>

> <span data-ttu-id="9975f-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="9975f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9975f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9975f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9975f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="9975f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9975f-107">Contém as propriedades de um conteúdo genérico MIME.</span><span class="sxs-lookup"><span data-stu-id="9975f-107">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="9975f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9975f-108">Properties</span></span>
|<span data-ttu-id="9975f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9975f-109">Property</span></span>|<span data-ttu-id="9975f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9975f-110">Type</span></span>|<span data-ttu-id="9975f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9975f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9975f-112">type</span><span class="sxs-lookup"><span data-stu-id="9975f-112">type</span></span>|<span data-ttu-id="9975f-113">String</span><span class="sxs-lookup"><span data-stu-id="9975f-113">String</span></span>|<span data-ttu-id="9975f-114">Indica o tipo de conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="9975f-114">Indicates the content mime type.</span></span>|
|<span data-ttu-id="9975f-115">valor</span><span class="sxs-lookup"><span data-stu-id="9975f-115">value</span></span>|<span data-ttu-id="9975f-116">Binária</span><span class="sxs-lookup"><span data-stu-id="9975f-116">Binary</span></span>|<span data-ttu-id="9975f-117">A matriz de byte que contém o conteúdo atual.</span><span class="sxs-lookup"><span data-stu-id="9975f-117">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9975f-118">Relações</span><span class="sxs-lookup"><span data-stu-id="9975f-118">Relationships</span></span>
<span data-ttu-id="9975f-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9975f-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9975f-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9975f-120">JSON Representation</span></span>
<span data-ttu-id="9975f-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9975f-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mimeContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mimeContent",
  "type": "String",
  "value": "binary"
}
```




