---
title: tipo de recurso de windowsKioskAzureADUser
description: A classe usada para identificar uma conta de usuário AzureAD para a configuração de quiosque
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 57b48bcdbac3f95da37704222cded29ba61cd32d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845882"
---
# <a name="windowskioskazureaduser-resource-type"></a><span data-ttu-id="a9835-103">tipo de recurso de windowsKioskAzureADUser</span><span class="sxs-lookup"><span data-stu-id="a9835-103">windowsKioskAzureADUser resource type</span></span>

> <span data-ttu-id="a9835-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a9835-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a9835-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a9835-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a9835-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a9835-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a9835-107">A classe usada para identificar uma conta de usuário AzureAD para a configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="a9835-107">The class used to identify an AzureAD user account for the kiosk configuration</span></span>

<span data-ttu-id="a9835-108">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="a9835-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a9835-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a9835-109">Properties</span></span>
|<span data-ttu-id="a9835-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9835-110">Property</span></span>|<span data-ttu-id="a9835-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9835-111">Type</span></span>|<span data-ttu-id="a9835-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9835-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9835-113">userId</span><span class="sxs-lookup"><span data-stu-id="a9835-113">userId</span></span>|<span data-ttu-id="a9835-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9835-114">String</span></span>|<span data-ttu-id="a9835-115">A ID do usuário AzureAD que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="a9835-115">The ID of the AzureAD user that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="a9835-116">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a9835-116">userPrincipalName</span></span>|<span data-ttu-id="a9835-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9835-117">String</span></span>|<span data-ttu-id="a9835-118">As contas de usuário que serão bloqueadas para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="a9835-118">The user accounts that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9835-119">Relações</span><span class="sxs-lookup"><span data-stu-id="a9835-119">Relationships</span></span>
<span data-ttu-id="a9835-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a9835-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a9835-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a9835-121">JSON Representation</span></span>
<span data-ttu-id="a9835-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a9835-122">Here is a JSON representation of the resource.</span></span>
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





