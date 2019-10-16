---
title: tipo de recurso mobileAppInstallTimeSettings
description: Contém propriedades usadas para determinar quando oferecer um aplicativo a dispositivos e quando instalar o aplicativo em dispositivos.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d99505990bb19789046521632441c4026a0ee404
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538711"
---
# <a name="mobileappinstalltimesettings-resource-type"></a><span data-ttu-id="67803-103">tipo de recurso mobileAppInstallTimeSettings</span><span class="sxs-lookup"><span data-stu-id="67803-103">mobileAppInstallTimeSettings resource type</span></span>

> <span data-ttu-id="67803-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="67803-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67803-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="67803-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67803-106">Contém propriedades usadas para determinar quando oferecer um aplicativo a dispositivos e quando instalar o aplicativo em dispositivos.</span><span class="sxs-lookup"><span data-stu-id="67803-106">Contains properties used to determine when to offer an app to devices and when to install the app on devices.</span></span>

## <a name="properties"></a><span data-ttu-id="67803-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="67803-107">Properties</span></span>
|<span data-ttu-id="67803-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67803-108">Property</span></span>|<span data-ttu-id="67803-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="67803-109">Type</span></span>|<span data-ttu-id="67803-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="67803-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67803-111">useLocalTime</span><span class="sxs-lookup"><span data-stu-id="67803-111">useLocalTime</span></span>|<span data-ttu-id="67803-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="67803-112">Boolean</span></span>|<span data-ttu-id="67803-113">Se a hora do dispositivo local ou a hora UTC deve ser usada ao determinar os horários disponíveis e prazos.</span><span class="sxs-lookup"><span data-stu-id="67803-113">Whether the local device time or UTC time should be used when determining the available and deadline times.</span></span>|
|<span data-ttu-id="67803-114">startDateTime</span><span class="sxs-lookup"><span data-stu-id="67803-114">startDateTime</span></span>|<span data-ttu-id="67803-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67803-115">DateTimeOffset</span></span>|<span data-ttu-id="67803-116">O horário em que o aplicativo deve estar disponível para instalação.</span><span class="sxs-lookup"><span data-stu-id="67803-116">The time at which the app should be available for installation.</span></span>|
|<span data-ttu-id="67803-117">deadlineDateTime</span><span class="sxs-lookup"><span data-stu-id="67803-117">deadlineDateTime</span></span>|<span data-ttu-id="67803-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67803-118">DateTimeOffset</span></span>|<span data-ttu-id="67803-119">O horário em que o aplicativo deve ser instalado.</span><span class="sxs-lookup"><span data-stu-id="67803-119">The time at which the app should be installed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="67803-120">Relações</span><span class="sxs-lookup"><span data-stu-id="67803-120">Relationships</span></span>
<span data-ttu-id="67803-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="67803-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="67803-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="67803-122">JSON Representation</span></span>
<span data-ttu-id="67803-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="67803-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppInstallTimeSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallTimeSettings",
  "useLocalTime": true,
  "startDateTime": "String (timestamp)",
  "deadlineDateTime": "String (timestamp)"
}
```



