---
title: Tipo de recurso keyValuePair
description: Par chave-valor para armazenar configurações personalizadas
author: tfitzmac
ms.openlocfilehash: f6438d97376d46f66e02026acc87c948ab2a91bb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329313"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="49869-103">Tipo de recurso keyValuePair</span><span class="sxs-lookup"><span data-stu-id="49869-103">keyValuePair resource type</span></span>

> <span data-ttu-id="49869-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="49869-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49869-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="49869-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="49869-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="49869-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="49869-107">Par chave-valor para armazenar configurações personalizadas</span><span class="sxs-lookup"><span data-stu-id="49869-107">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="49869-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="49869-108">Properties</span></span>
|<span data-ttu-id="49869-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49869-109">Property</span></span>|<span data-ttu-id="49869-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="49869-110">Type</span></span>|<span data-ttu-id="49869-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="49869-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49869-112">name</span><span class="sxs-lookup"><span data-stu-id="49869-112">name</span></span>|<span data-ttu-id="49869-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49869-113">String</span></span>|<span data-ttu-id="49869-114">Nome deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="49869-114">Name for this key-value pair</span></span>|
|<span data-ttu-id="49869-115">valor</span><span class="sxs-lookup"><span data-stu-id="49869-115">value</span></span>|<span data-ttu-id="49869-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49869-116">String</span></span>|<span data-ttu-id="49869-117">Valor deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="49869-117">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="49869-118">Relações</span><span class="sxs-lookup"><span data-stu-id="49869-118">Relationships</span></span>
<span data-ttu-id="49869-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="49869-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="49869-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="49869-120">JSON Representation</span></span>
<span data-ttu-id="49869-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="49869-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValuePair",
  "name": "String",
  "value": "String"
}
```





