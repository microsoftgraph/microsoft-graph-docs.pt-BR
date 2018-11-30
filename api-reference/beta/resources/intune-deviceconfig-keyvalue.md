---
title: tipo de recurso keyValue
description: Definição do valor da chave.
ms.openlocfilehash: 7279b48243139b9234b737ceb7d7fb1ad7232451
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035571"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="ed9b0-103">tipo de recurso keyValue</span><span class="sxs-lookup"><span data-stu-id="ed9b0-103">keyValue resource type</span></span>

> <span data-ttu-id="ed9b0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ed9b0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed9b0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ed9b0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ed9b0-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ed9b0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed9b0-107">Definição do valor da chave.</span><span class="sxs-lookup"><span data-stu-id="ed9b0-107">Key Value definition.</span></span>
## <a name="properties"></a><span data-ttu-id="ed9b0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed9b0-108">Properties</span></span>
|<span data-ttu-id="ed9b0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed9b0-109">Property</span></span>|<span data-ttu-id="ed9b0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed9b0-110">Type</span></span>|<span data-ttu-id="ed9b0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed9b0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed9b0-112">key</span><span class="sxs-lookup"><span data-stu-id="ed9b0-112">key</span></span>|<span data-ttu-id="ed9b0-113">String</span><span class="sxs-lookup"><span data-stu-id="ed9b0-113">String</span></span>|<span data-ttu-id="ed9b0-114">Chave.</span><span class="sxs-lookup"><span data-stu-id="ed9b0-114">Key.</span></span>|
|<span data-ttu-id="ed9b0-115">valor</span><span class="sxs-lookup"><span data-stu-id="ed9b0-115">value</span></span>|<span data-ttu-id="ed9b0-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed9b0-116">String</span></span>|<span data-ttu-id="ed9b0-117">Valor.</span><span class="sxs-lookup"><span data-stu-id="ed9b0-117">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed9b0-118">Relações</span><span class="sxs-lookup"><span data-stu-id="ed9b0-118">Relationships</span></span>
<span data-ttu-id="ed9b0-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ed9b0-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ed9b0-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed9b0-120">JSON Representation</span></span>
<span data-ttu-id="ed9b0-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ed9b0-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValue",
  "key": "String",
  "value": "String"
}
```





