---
title: tipo de recurso windowsKioskAzureADUser
description: A classe usada para identificar uma conta de usuário do AzureAD para a configuração do quiosque
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4b946007fd8b16d2f6c016025d58e07392b6c1a9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690655"
---
# <a name="windowskioskazureaduser-resource-type"></a><span data-ttu-id="811d0-103">tipo de recurso windowsKioskAzureADUser</span><span class="sxs-lookup"><span data-stu-id="811d0-103">windowsKioskAzureADUser resource type</span></span>

<span data-ttu-id="811d0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="811d0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="811d0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="811d0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="811d0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="811d0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="811d0-107">A classe usada para identificar uma conta de usuário do AzureAD para a configuração do quiosque</span><span class="sxs-lookup"><span data-stu-id="811d0-107">The class used to identify an AzureAD user account for the kiosk configuration</span></span>


<span data-ttu-id="811d0-108">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="811d0-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="811d0-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="811d0-109">Properties</span></span>
|<span data-ttu-id="811d0-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="811d0-110">Property</span></span>|<span data-ttu-id="811d0-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="811d0-111">Type</span></span>|<span data-ttu-id="811d0-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="811d0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="811d0-113">userId</span><span class="sxs-lookup"><span data-stu-id="811d0-113">userId</span></span>|<span data-ttu-id="811d0-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="811d0-114">String</span></span>|<span data-ttu-id="811d0-115">A ID do usuário do AzureAD que será bloqueada para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="811d0-115">The ID of the AzureAD user that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="811d0-116">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="811d0-116">userPrincipalName</span></span>|<span data-ttu-id="811d0-117">String</span><span class="sxs-lookup"><span data-stu-id="811d0-117">String</span></span>|<span data-ttu-id="811d0-118">As contas de usuário que serão bloqueadas para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="811d0-118">The user accounts that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="811d0-119">Relações</span><span class="sxs-lookup"><span data-stu-id="811d0-119">Relationships</span></span>
<span data-ttu-id="811d0-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="811d0-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="811d0-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="811d0-121">JSON Representation</span></span>
<span data-ttu-id="811d0-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="811d0-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADUser",
  "userId": "String",
  "userPrincipalName": "String"
}
```





