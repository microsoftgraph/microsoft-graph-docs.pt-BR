---
title: tipo de recurso adminConsent
description: Informações de consentimento do administrador.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7f13e8abbaf20f57e94923918a4e5c2bb5bcf9b9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968607"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="012b2-103">tipo de recurso adminConsent</span><span class="sxs-lookup"><span data-stu-id="012b2-103">adminConsent resource type</span></span>

> <span data-ttu-id="012b2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="012b2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="012b2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="012b2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="012b2-106">Informações de consentimento do administrador.</span><span class="sxs-lookup"><span data-stu-id="012b2-106">Admin consent information.</span></span>

## <a name="properties"></a><span data-ttu-id="012b2-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="012b2-107">Properties</span></span>
|<span data-ttu-id="012b2-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="012b2-108">Property</span></span>|<span data-ttu-id="012b2-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="012b2-109">Type</span></span>|<span data-ttu-id="012b2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="012b2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="012b2-111">shareAPNSData</span><span class="sxs-lookup"><span data-stu-id="012b2-111">shareAPNSData</span></span>|[<span data-ttu-id="012b2-112">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="012b2-112">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="012b2-113">O estado de consentimento do administrador do compartilhamento de dados de usuário e de dispositivo para a Apple.</span><span class="sxs-lookup"><span data-stu-id="012b2-113">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="012b2-114">Os valores possíveis são: `notConfigured`, `granted`, `notGranted`.</span><span class="sxs-lookup"><span data-stu-id="012b2-114">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="012b2-115">Relações</span><span class="sxs-lookup"><span data-stu-id="012b2-115">Relationships</span></span>
<span data-ttu-id="012b2-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="012b2-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="012b2-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="012b2-117">JSON Representation</span></span>
<span data-ttu-id="012b2-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="012b2-118">Here is a JSON representation of the resource.</span></span>
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





