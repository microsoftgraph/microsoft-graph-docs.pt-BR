---
title: tipo de recurso keyValue
description: Definição do valor da chave.
author: tfitzmac
ms.openlocfilehash: 5e5754657e679f3a703c2b5dec7cea36d1bad860
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302636"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="3c93c-103">tipo de recurso keyValue</span><span class="sxs-lookup"><span data-stu-id="3c93c-103">keyValue resource type</span></span>

> <span data-ttu-id="3c93c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3c93c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c93c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3c93c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3c93c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3c93c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c93c-107">Definição do valor da chave.</span><span class="sxs-lookup"><span data-stu-id="3c93c-107">Key Value definition.</span></span>
## <a name="properties"></a><span data-ttu-id="3c93c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3c93c-108">Properties</span></span>
|<span data-ttu-id="3c93c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c93c-109">Property</span></span>|<span data-ttu-id="3c93c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c93c-110">Type</span></span>|<span data-ttu-id="3c93c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c93c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c93c-112">key</span><span class="sxs-lookup"><span data-stu-id="3c93c-112">key</span></span>|<span data-ttu-id="3c93c-113">String</span><span class="sxs-lookup"><span data-stu-id="3c93c-113">String</span></span>|<span data-ttu-id="3c93c-114">Chave.</span><span class="sxs-lookup"><span data-stu-id="3c93c-114">Key.</span></span>|
|<span data-ttu-id="3c93c-115">valor</span><span class="sxs-lookup"><span data-stu-id="3c93c-115">value</span></span>|<span data-ttu-id="3c93c-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c93c-116">String</span></span>|<span data-ttu-id="3c93c-117">Valor.</span><span class="sxs-lookup"><span data-stu-id="3c93c-117">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c93c-118">Relações</span><span class="sxs-lookup"><span data-stu-id="3c93c-118">Relationships</span></span>
<span data-ttu-id="3c93c-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3c93c-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3c93c-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3c93c-120">JSON Representation</span></span>
<span data-ttu-id="3c93c-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3c93c-121">Here is a JSON representation of the resource.</span></span>
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





