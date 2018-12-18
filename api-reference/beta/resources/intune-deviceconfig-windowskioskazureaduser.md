---
title: tipo de recurso de windowsKioskAzureADUser
description: A classe usada para identificar uma conta de usuário AzureAD para a configuração de quiosque
author: tfitzmac
ms.openlocfilehash: e4048b4cbea592af350af20bf433ca00ac6d4980
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330069"
---
# <a name="windowskioskazureaduser-resource-type"></a><span data-ttu-id="41c86-103">tipo de recurso de windowsKioskAzureADUser</span><span class="sxs-lookup"><span data-stu-id="41c86-103">windowsKioskAzureADUser resource type</span></span>

> <span data-ttu-id="41c86-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="41c86-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="41c86-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="41c86-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="41c86-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="41c86-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="41c86-107">A classe usada para identificar uma conta de usuário AzureAD para a configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="41c86-107">The class used to identify an AzureAD user account for the kiosk configuration</span></span>

<span data-ttu-id="41c86-108">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="41c86-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="41c86-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="41c86-109">Properties</span></span>
|<span data-ttu-id="41c86-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41c86-110">Property</span></span>|<span data-ttu-id="41c86-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="41c86-111">Type</span></span>|<span data-ttu-id="41c86-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="41c86-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41c86-113">userId</span><span class="sxs-lookup"><span data-stu-id="41c86-113">userId</span></span>|<span data-ttu-id="41c86-114">String</span><span class="sxs-lookup"><span data-stu-id="41c86-114">String</span></span>|<span data-ttu-id="41c86-115">A ID do usuário AzureAD que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="41c86-115">The ID of the AzureAD user that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="41c86-116">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="41c86-116">userPrincipalName</span></span>|<span data-ttu-id="41c86-117">String</span><span class="sxs-lookup"><span data-stu-id="41c86-117">String</span></span>|<span data-ttu-id="41c86-118">As contas de usuário que serão bloqueadas para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="41c86-118">The user accounts that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="41c86-119">Relações</span><span class="sxs-lookup"><span data-stu-id="41c86-119">Relationships</span></span>
<span data-ttu-id="41c86-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="41c86-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="41c86-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="41c86-121">JSON Representation</span></span>
<span data-ttu-id="41c86-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="41c86-122">Here is a JSON representation of the resource.</span></span>
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





