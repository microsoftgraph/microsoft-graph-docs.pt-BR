---
title: Tipo de recurso azureADDeviceRegistrationError
description: Um erro no processo de registro de um dispositivo do Azure AD que impede o serviço de registrar o dispositivo no gerenciamento de atualizações ou implantar conteúdo no dispositivo.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 1d08ab96d5298c70f34acf89e3c6c4605d9df0a1
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067800"
---
# <a name="azureaddeviceregistrationerror-resource-type"></a><span data-ttu-id="a51d7-103">Tipo de recurso azureADDeviceRegistrationError</span><span class="sxs-lookup"><span data-stu-id="a51d7-103">azureADDeviceRegistrationError resource type</span></span>

<span data-ttu-id="a51d7-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="a51d7-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a51d7-105">Um erro no processo de registro de um dispositivo [do Azure AD](../resources/windowsupdates-azureaddevice.md) que impede o serviço de registrar o dispositivo no gerenciamento de atualizações ou implantar conteúdo no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a51d7-105">An error in the registration process of an [Azure AD device](../resources/windowsupdates-azureaddevice.md) that prevents the service from enrolling the device in update management or deploying content to the device.</span></span>

<span data-ttu-id="a51d7-106">Herda de [updatableAssetError](../resources/windowsupdates-updatableasseterror.md).</span><span class="sxs-lookup"><span data-stu-id="a51d7-106">Inherits from [updatableAssetError](../resources/windowsupdates-updatableasseterror.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a51d7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a51d7-107">Properties</span></span>
|<span data-ttu-id="a51d7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a51d7-108">Property</span></span>|<span data-ttu-id="a51d7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a51d7-109">Type</span></span>|<span data-ttu-id="a51d7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a51d7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a51d7-111">motivo</span><span class="sxs-lookup"><span data-stu-id="a51d7-111">reason</span></span>|<span data-ttu-id="a51d7-112">microsoft.graph.windowsUpdates.azureADDeviceRegistrationErrorReason</span><span class="sxs-lookup"><span data-stu-id="a51d7-112">microsoft.graph.windowsUpdates.azureADDeviceRegistrationErrorReason</span></span>|<span data-ttu-id="a51d7-113">O motivo pelo qual o registro encontrou um erro.</span><span class="sxs-lookup"><span data-stu-id="a51d7-113">The reason why the registration encountered an error.</span></span> <span data-ttu-id="a51d7-114">Os valores possíveis são: `invalidGlobalDeviceId`, `invalidAzureADDeviceId`, `missingTrustType`, `invalidAzureADJoin`.</span><span class="sxs-lookup"><span data-stu-id="a51d7-114">Possible values are: `invalidGlobalDeviceId`, `invalidAzureADDeviceId`, `missingTrustType`, `invalidAzureADJoin`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a51d7-115">Relações</span><span class="sxs-lookup"><span data-stu-id="a51d7-115">Relationships</span></span>
<span data-ttu-id="a51d7-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a51d7-116">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a51d7-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a51d7-117">JSON representation</span></span>
<span data-ttu-id="a51d7-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a51d7-118">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.azureADDeviceRegistrationError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.azureADDeviceRegistrationError",
  "reason": "String"
}
```

