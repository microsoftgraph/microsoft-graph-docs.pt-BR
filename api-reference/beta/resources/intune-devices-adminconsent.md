---
title: tipo de recurso adminConsent
description: Informações de consentimento do administrador.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aaac2bb11d90f1e6fec52fae0c17f374c33868ce
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943365"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="e00a9-103">tipo de recurso adminConsent</span><span class="sxs-lookup"><span data-stu-id="e00a9-103">adminConsent resource type</span></span>

> <span data-ttu-id="e00a9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e00a9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e00a9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e00a9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e00a9-106">Informações de consentimento do administrador.</span><span class="sxs-lookup"><span data-stu-id="e00a9-106">Admin consent information.</span></span>

## <a name="properties"></a><span data-ttu-id="e00a9-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e00a9-107">Properties</span></span>
|<span data-ttu-id="e00a9-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e00a9-108">Property</span></span>|<span data-ttu-id="e00a9-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e00a9-109">Type</span></span>|<span data-ttu-id="e00a9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e00a9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e00a9-111">shareAPNSData</span><span class="sxs-lookup"><span data-stu-id="e00a9-111">shareAPNSData</span></span>|[<span data-ttu-id="e00a9-112">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="e00a9-112">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="e00a9-113">O estado de consentimento do administrador do compartilhamento de dados de usuário e de dispositivo para a Apple.</span><span class="sxs-lookup"><span data-stu-id="e00a9-113">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="e00a9-114">Os valores possíveis são: `notConfigured`, `granted`, `notGranted`.</span><span class="sxs-lookup"><span data-stu-id="e00a9-114">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e00a9-115">Relações</span><span class="sxs-lookup"><span data-stu-id="e00a9-115">Relationships</span></span>
<span data-ttu-id="e00a9-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e00a9-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e00a9-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e00a9-117">JSON Representation</span></span>
<span data-ttu-id="e00a9-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e00a9-118">Here is a JSON representation of the resource.</span></span>
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




