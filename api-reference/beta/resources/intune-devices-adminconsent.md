---
title: tipo de recurso de adminConsent
description: Informações de consentimento do administrador.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4b6b2d9a8c32c9a1ce7e8587ebe853f7646b703a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815573"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="ed314-103">tipo de recurso de adminConsent</span><span class="sxs-lookup"><span data-stu-id="ed314-103">adminConsent resource type</span></span>

> <span data-ttu-id="ed314-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ed314-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed314-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ed314-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ed314-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ed314-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed314-107">Informações de consentimento do administrador.</span><span class="sxs-lookup"><span data-stu-id="ed314-107">Admin consent information.</span></span>
## <a name="properties"></a><span data-ttu-id="ed314-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed314-108">Properties</span></span>
|<span data-ttu-id="ed314-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed314-109">Property</span></span>|<span data-ttu-id="ed314-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed314-110">Type</span></span>|<span data-ttu-id="ed314-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed314-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed314-112">shareAPNSData</span><span class="sxs-lookup"><span data-stu-id="ed314-112">shareAPNSData</span></span>|[<span data-ttu-id="ed314-113">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="ed314-113">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="ed314-114">O estado de consentimento de admin de compartilhamento de usuário e dados de dispositivo para Apple.</span><span class="sxs-lookup"><span data-stu-id="ed314-114">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="ed314-115">Os valores possíveis são: `notConfigured`, `granted`, `notGranted`.</span><span class="sxs-lookup"><span data-stu-id="ed314-115">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed314-116">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="ed314-116">Relationships</span></span>
<span data-ttu-id="ed314-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ed314-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ed314-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed314-118">JSON Representation</span></span>
<span data-ttu-id="ed314-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ed314-119">Here is a JSON representation of the resource.</span></span>
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





