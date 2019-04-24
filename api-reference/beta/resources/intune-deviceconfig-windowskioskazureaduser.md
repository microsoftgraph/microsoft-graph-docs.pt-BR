---
title: tipo de recurso windowsKioskAzureADUser
description: A classe usada para identificar uma conta de usuário do AzureAD para a configuração do quiosque
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 93a47ba1bafe8f2070eedb028cb0eaa64808d03d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522486"
---
# <a name="windowskioskazureaduser-resource-type"></a><span data-ttu-id="35d15-103">tipo de recurso windowsKioskAzureADUser</span><span class="sxs-lookup"><span data-stu-id="35d15-103">windowsKioskAzureADUser resource type</span></span>

> <span data-ttu-id="35d15-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="35d15-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35d15-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="35d15-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35d15-106">A classe usada para identificar uma conta de usuário do AzureAD para a configuração do quiosque</span><span class="sxs-lookup"><span data-stu-id="35d15-106">The class used to identify an AzureAD user account for the kiosk configuration</span></span>


<span data-ttu-id="35d15-107">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="35d15-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="35d15-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="35d15-108">Properties</span></span>
|<span data-ttu-id="35d15-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35d15-109">Property</span></span>|<span data-ttu-id="35d15-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="35d15-110">Type</span></span>|<span data-ttu-id="35d15-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="35d15-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35d15-112">userId</span><span class="sxs-lookup"><span data-stu-id="35d15-112">userId</span></span>|<span data-ttu-id="35d15-113">String</span><span class="sxs-lookup"><span data-stu-id="35d15-113">String</span></span>|<span data-ttu-id="35d15-114">A ID do usuário do AzureAD que será bloqueada para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="35d15-114">The ID of the AzureAD user that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="35d15-115">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="35d15-115">userPrincipalName</span></span>|<span data-ttu-id="35d15-116">String</span><span class="sxs-lookup"><span data-stu-id="35d15-116">String</span></span>|<span data-ttu-id="35d15-117">As contas de usuário que serão bloqueadas para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="35d15-117">The user accounts that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="35d15-118">Relações</span><span class="sxs-lookup"><span data-stu-id="35d15-118">Relationships</span></span>
<span data-ttu-id="35d15-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="35d15-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35d15-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="35d15-120">JSON Representation</span></span>
<span data-ttu-id="35d15-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="35d15-121">Here is a JSON representation of the resource.</span></span>
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





