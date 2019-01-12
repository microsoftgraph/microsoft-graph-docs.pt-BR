---
title: tipo de recurso de adminConsent
description: Informações de consentimento do administrador.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 428729ff9a8a8ee5deb64c537922cb7a0417ba2e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962125"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="ad863-103">tipo de recurso de adminConsent</span><span class="sxs-lookup"><span data-stu-id="ad863-103">adminConsent resource type</span></span>

> <span data-ttu-id="ad863-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ad863-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad863-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ad863-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ad863-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ad863-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad863-107">Informações de consentimento do administrador.</span><span class="sxs-lookup"><span data-stu-id="ad863-107">Admin consent information.</span></span>
## <a name="properties"></a><span data-ttu-id="ad863-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ad863-108">Properties</span></span>
|<span data-ttu-id="ad863-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ad863-109">Property</span></span>|<span data-ttu-id="ad863-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad863-110">Type</span></span>|<span data-ttu-id="ad863-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad863-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad863-112">shareAPNSData</span><span class="sxs-lookup"><span data-stu-id="ad863-112">shareAPNSData</span></span>|[<span data-ttu-id="ad863-113">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="ad863-113">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="ad863-114">O estado de consentimento de admin de compartilhamento de usuário e dados de dispositivo para Apple.</span><span class="sxs-lookup"><span data-stu-id="ad863-114">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="ad863-115">Os valores possíveis são: `notConfigured`, `granted`, `notGranted`.</span><span class="sxs-lookup"><span data-stu-id="ad863-115">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad863-116">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="ad863-116">Relationships</span></span>
<span data-ttu-id="ad863-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ad863-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ad863-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ad863-118">JSON Representation</span></span>
<span data-ttu-id="ad863-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ad863-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.adminConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminConsent",
  "shareAPNSData": "String"
}
```





