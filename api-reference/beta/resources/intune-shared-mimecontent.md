---
title: Tipo de recurso mimeContent
description: Contém as propriedades de um conteúdo genérico MIME.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ee38eee9100982f6dc5f22315af480a783cc4252
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962118"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="9c6c4-103">Tipo de recurso mimeContent</span><span class="sxs-lookup"><span data-stu-id="9c6c4-103">mimeContent resource type</span></span>

> <span data-ttu-id="9c6c4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9c6c4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9c6c4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9c6c4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9c6c4-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9c6c4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9c6c4-107">Contém as propriedades de um conteúdo genérico MIME.</span><span class="sxs-lookup"><span data-stu-id="9c6c4-107">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="9c6c4-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9c6c4-108">Properties</span></span>
|<span data-ttu-id="9c6c4-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c6c4-109">Property</span></span>|<span data-ttu-id="9c6c4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c6c4-110">Type</span></span>|<span data-ttu-id="9c6c4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c6c4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c6c4-112">type</span><span class="sxs-lookup"><span data-stu-id="9c6c4-112">type</span></span>|<span data-ttu-id="9c6c4-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c6c4-113">String</span></span>|<span data-ttu-id="9c6c4-114">Indica o tipo de conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="9c6c4-114">Indicates the content mime type.</span></span>|
|<span data-ttu-id="9c6c4-115">valor</span><span class="sxs-lookup"><span data-stu-id="9c6c4-115">value</span></span>|<span data-ttu-id="9c6c4-116">Binária</span><span class="sxs-lookup"><span data-stu-id="9c6c4-116">Binary</span></span>|<span data-ttu-id="9c6c4-117">A matriz de byte que contém o conteúdo atual.</span><span class="sxs-lookup"><span data-stu-id="9c6c4-117">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c6c4-118">Relações</span><span class="sxs-lookup"><span data-stu-id="9c6c4-118">Relationships</span></span>
<span data-ttu-id="9c6c4-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9c6c4-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9c6c4-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9c6c4-120">JSON Representation</span></span>
<span data-ttu-id="9c6c4-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9c6c4-121">Here is a JSON representation of the resource.</span></span>
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





