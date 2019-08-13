---
title: tipo de recurso windowsKioskAzureADUser
description: A classe usada para identificar uma conta de usuário do AzureAD para a configuração do quiosque
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a7f2f72fc9d7ed6b0e1209bcff2fa81a806c7e21
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370927"
---
# <a name="windowskioskazureaduser-resource-type"></a><span data-ttu-id="15e55-103">tipo de recurso windowsKioskAzureADUser</span><span class="sxs-lookup"><span data-stu-id="15e55-103">windowsKioskAzureADUser resource type</span></span>

> <span data-ttu-id="15e55-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="15e55-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15e55-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="15e55-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15e55-106">A classe usada para identificar uma conta de usuário do AzureAD para a configuração do quiosque</span><span class="sxs-lookup"><span data-stu-id="15e55-106">The class used to identify an AzureAD user account for the kiosk configuration</span></span>


<span data-ttu-id="15e55-107">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="15e55-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="15e55-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="15e55-108">Properties</span></span>
|<span data-ttu-id="15e55-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="15e55-109">Property</span></span>|<span data-ttu-id="15e55-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="15e55-110">Type</span></span>|<span data-ttu-id="15e55-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="15e55-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15e55-112">userId</span><span class="sxs-lookup"><span data-stu-id="15e55-112">userId</span></span>|<span data-ttu-id="15e55-113">String</span><span class="sxs-lookup"><span data-stu-id="15e55-113">String</span></span>|<span data-ttu-id="15e55-114">A ID do usuário do AzureAD que será bloqueada para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="15e55-114">The ID of the AzureAD user that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="15e55-115">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="15e55-115">userPrincipalName</span></span>|<span data-ttu-id="15e55-116">String</span><span class="sxs-lookup"><span data-stu-id="15e55-116">String</span></span>|<span data-ttu-id="15e55-117">As contas de usuário que serão bloqueadas para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="15e55-117">The user accounts that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="15e55-118">Relações</span><span class="sxs-lookup"><span data-stu-id="15e55-118">Relationships</span></span>
<span data-ttu-id="15e55-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="15e55-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="15e55-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="15e55-120">JSON Representation</span></span>
<span data-ttu-id="15e55-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="15e55-121">Here is a JSON representation of the resource.</span></span>
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



