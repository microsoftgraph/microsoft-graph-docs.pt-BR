---
title: tipo de recurso extendedKeyUsage
description: Definição de uso de chave estendida personalizada
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1487d217693135e26df99d4d72491abac4123ba7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173287"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="1ddde-103">tipo de recurso extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="1ddde-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="1ddde-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1ddde-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ddde-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1ddde-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ddde-106">Definição de uso de chave estendida personalizada</span><span class="sxs-lookup"><span data-stu-id="1ddde-106">Custom Extended Key Usage definition</span></span>

## <a name="properties"></a><span data-ttu-id="1ddde-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1ddde-107">Properties</span></span>
|<span data-ttu-id="1ddde-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ddde-108">Property</span></span>|<span data-ttu-id="1ddde-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ddde-109">Type</span></span>|<span data-ttu-id="1ddde-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ddde-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ddde-111">name</span><span class="sxs-lookup"><span data-stu-id="1ddde-111">name</span></span>|<span data-ttu-id="1ddde-112">String</span><span class="sxs-lookup"><span data-stu-id="1ddde-112">String</span></span>|<span data-ttu-id="1ddde-113">Nome estendido do uso de chave</span><span class="sxs-lookup"><span data-stu-id="1ddde-113">Extended Key Usage Name</span></span>|
|<span data-ttu-id="1ddde-114">objectIdentifier</span><span class="sxs-lookup"><span data-stu-id="1ddde-114">objectIdentifier</span></span>|<span data-ttu-id="1ddde-115">String</span><span class="sxs-lookup"><span data-stu-id="1ddde-115">String</span></span>|<span data-ttu-id="1ddde-116">Identificador de objeto de uso estendido de chave</span><span class="sxs-lookup"><span data-stu-id="1ddde-116">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ddde-117">Relações</span><span class="sxs-lookup"><span data-stu-id="1ddde-117">Relationships</span></span>
<span data-ttu-id="1ddde-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1ddde-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ddde-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1ddde-119">JSON Representation</span></span>
<span data-ttu-id="1ddde-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1ddde-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.extendedKeyUsage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.extendedKeyUsage",
  "name": "String",
  "objectIdentifier": "String"
}
```




