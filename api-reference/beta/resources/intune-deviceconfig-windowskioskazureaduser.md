---
title: tipo de recurso de windowsKioskAzureADUser
description: A classe usada para identificar uma conta de usuário AzureAD para a configuração de quiosque
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 08c5b53e8e208abac2801146ff70df6023eaedff
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420182"
---
# <a name="windowskioskazureaduser-resource-type"></a><span data-ttu-id="13c8a-103">tipo de recurso de windowsKioskAzureADUser</span><span class="sxs-lookup"><span data-stu-id="13c8a-103">windowsKioskAzureADUser resource type</span></span>

> <span data-ttu-id="13c8a-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="13c8a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="13c8a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="13c8a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="13c8a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="13c8a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13c8a-107">A classe usada para identificar uma conta de usuário AzureAD para a configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="13c8a-107">The class used to identify an AzureAD user account for the kiosk configuration</span></span>


<span data-ttu-id="13c8a-108">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="13c8a-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="13c8a-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="13c8a-109">Properties</span></span>
|<span data-ttu-id="13c8a-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13c8a-110">Property</span></span>|<span data-ttu-id="13c8a-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="13c8a-111">Type</span></span>|<span data-ttu-id="13c8a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="13c8a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13c8a-113">userId</span><span class="sxs-lookup"><span data-stu-id="13c8a-113">userId</span></span>|<span data-ttu-id="13c8a-114">String</span><span class="sxs-lookup"><span data-stu-id="13c8a-114">String</span></span>|<span data-ttu-id="13c8a-115">A ID do usuário AzureAD que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="13c8a-115">The ID of the AzureAD user that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="13c8a-116">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="13c8a-116">userPrincipalName</span></span>|<span data-ttu-id="13c8a-117">String</span><span class="sxs-lookup"><span data-stu-id="13c8a-117">String</span></span>|<span data-ttu-id="13c8a-118">As contas de usuário que serão bloqueadas para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="13c8a-118">The user accounts that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="13c8a-119">Relações</span><span class="sxs-lookup"><span data-stu-id="13c8a-119">Relationships</span></span>
<span data-ttu-id="13c8a-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="13c8a-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13c8a-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="13c8a-121">JSON Representation</span></span>
<span data-ttu-id="13c8a-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="13c8a-122">Here is a JSON representation of the resource.</span></span>
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




