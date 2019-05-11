---
title: tipo de recurso extendedKeyUsage
description: Definição de uso de chave estendida personalizada
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 36752e9a2f86e68bd4ada1a342dc174726a684c7
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946949"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="54fd1-103">tipo de recurso extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="54fd1-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="54fd1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="54fd1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54fd1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="54fd1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54fd1-106">Definição de uso de chave estendida personalizada</span><span class="sxs-lookup"><span data-stu-id="54fd1-106">Custom Extended Key Usage definition</span></span>

## <a name="properties"></a><span data-ttu-id="54fd1-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="54fd1-107">Properties</span></span>
|<span data-ttu-id="54fd1-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54fd1-108">Property</span></span>|<span data-ttu-id="54fd1-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="54fd1-109">Type</span></span>|<span data-ttu-id="54fd1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="54fd1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54fd1-111">nome</span><span class="sxs-lookup"><span data-stu-id="54fd1-111">name</span></span>|<span data-ttu-id="54fd1-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54fd1-112">String</span></span>|<span data-ttu-id="54fd1-113">Nome estendido do uso de chave</span><span class="sxs-lookup"><span data-stu-id="54fd1-113">Extended Key Usage Name</span></span>|
|<span data-ttu-id="54fd1-114">objectidentifier</span><span class="sxs-lookup"><span data-stu-id="54fd1-114">objectIdentifier</span></span>|<span data-ttu-id="54fd1-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54fd1-115">String</span></span>|<span data-ttu-id="54fd1-116">Identificador de objeto de uso estendido de chave</span><span class="sxs-lookup"><span data-stu-id="54fd1-116">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="54fd1-117">Relações</span><span class="sxs-lookup"><span data-stu-id="54fd1-117">Relationships</span></span>
<span data-ttu-id="54fd1-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="54fd1-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="54fd1-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="54fd1-119">JSON Representation</span></span>
<span data-ttu-id="54fd1-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="54fd1-120">Here is a JSON representation of the resource.</span></span>
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




