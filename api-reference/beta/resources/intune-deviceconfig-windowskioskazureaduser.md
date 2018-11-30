---
title: tipo de recurso de windowsKioskAzureADUser
description: A classe usada para identificar uma conta de usuário AzureAD para a configuração de quiosque
ms.openlocfilehash: 22e71ab10ac7fb755050e8d6e5d19568bef2fae8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036323"
---
# <a name="windowskioskazureaduser-resource-type"></a><span data-ttu-id="eb26d-103">tipo de recurso de windowsKioskAzureADUser</span><span class="sxs-lookup"><span data-stu-id="eb26d-103">windowsKioskAzureADUser resource type</span></span>

> <span data-ttu-id="eb26d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="eb26d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eb26d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="eb26d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eb26d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="eb26d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eb26d-107">A classe usada para identificar uma conta de usuário AzureAD para a configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="eb26d-107">The class used to identify an AzureAD user account for the kiosk configuration</span></span>

<span data-ttu-id="eb26d-108">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="eb26d-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="eb26d-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eb26d-109">Properties</span></span>
|<span data-ttu-id="eb26d-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb26d-110">Property</span></span>|<span data-ttu-id="eb26d-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb26d-111">Type</span></span>|<span data-ttu-id="eb26d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb26d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb26d-113">userId</span><span class="sxs-lookup"><span data-stu-id="eb26d-113">userId</span></span>|<span data-ttu-id="eb26d-114">String</span><span class="sxs-lookup"><span data-stu-id="eb26d-114">String</span></span>|<span data-ttu-id="eb26d-115">A ID do usuário AzureAD que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="eb26d-115">The ID of the AzureAD user that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="eb26d-116">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="eb26d-116">userPrincipalName</span></span>|<span data-ttu-id="eb26d-117">String</span><span class="sxs-lookup"><span data-stu-id="eb26d-117">String</span></span>|<span data-ttu-id="eb26d-118">As contas de usuário que serão bloqueadas para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="eb26d-118">The user accounts that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb26d-119">Relações</span><span class="sxs-lookup"><span data-stu-id="eb26d-119">Relationships</span></span>
<span data-ttu-id="eb26d-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eb26d-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="eb26d-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eb26d-121">JSON Representation</span></span>
<span data-ttu-id="eb26d-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eb26d-122">Here is a JSON representation of the resource.</span></span>
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





