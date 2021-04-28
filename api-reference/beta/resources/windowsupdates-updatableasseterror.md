---
title: tipo de recurso updatableAssetError
description: Um tipo abstrato que representa um erro que impede o serviço de implantação de registrar um azureADDevice no gerenciamento de atualizações ou implantar conteúdo no dispositivo
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 4d4375be68aea6dd4cb27c7ae8b78aaf86a2edf1
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067235"
---
# <a name="updatableasseterror-resource-type"></a><span data-ttu-id="ec743-103">tipo de recurso updatableAssetError</span><span class="sxs-lookup"><span data-stu-id="ec743-103">updatableAssetError resource type</span></span>

<span data-ttu-id="ec743-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="ec743-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec743-105">Um tipo abstrato que representa um erro que impede o serviço de implantação de registrar um [azureADDevice](../resources/windowsupdates-azureaddevice.md) no gerenciamento de atualizações ou implantar conteúdo no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ec743-105">An abstract type that represents an error which prevents the deployment service from enrolling an [azureADDevice](../resources/windowsupdates-azureaddevice.md) in update management, or deploying content to the device.</span></span> 

<span data-ttu-id="ec743-106">Todos os erros de ativo atualizáveis são do tipo derivado, [azureADDeviceRegistrationError](../resources/windowsupdates-azureaddeviceregistrationerror.md).</span><span class="sxs-lookup"><span data-stu-id="ec743-106">All updatable asset errors are of the derived type, [azureADDeviceRegistrationError](../resources/windowsupdates-azureaddeviceregistrationerror.md).</span></span>


## <a name="properties"></a><span data-ttu-id="ec743-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ec743-107">Properties</span></span>
<span data-ttu-id="ec743-108">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ec743-108">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="ec743-109">Relações</span><span class="sxs-lookup"><span data-stu-id="ec743-109">Relationships</span></span>
<span data-ttu-id="ec743-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ec743-110">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ec743-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ec743-111">JSON representation</span></span>
<span data-ttu-id="ec743-112">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ec743-112">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.updatableAssetError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetError"
}
```

