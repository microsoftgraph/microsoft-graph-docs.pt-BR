---
title: Tipo de recurso deleteUserFromSharedAppleDeviceActionResult
description: Resultado de ação de excluir o usuário do dispositivo compartilhado da Apple
ms.openlocfilehash: 5ed6d7b8c07c28dce5ee8cc830a9e86bcdcafa1b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035777"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="b4ccd-103">Tipo de recurso deleteUserFromSharedAppleDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="b4ccd-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="b4ccd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b4ccd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b4ccd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b4ccd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b4ccd-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b4ccd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4ccd-107">Resultado de ação de excluir o usuário do dispositivo compartilhado da Apple</span><span class="sxs-lookup"><span data-stu-id="b4ccd-107">Delete user from shared apple device action result</span></span>

<span data-ttu-id="b4ccd-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b4ccd-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b4ccd-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b4ccd-109">Properties</span></span>
|<span data-ttu-id="b4ccd-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4ccd-110">Property</span></span>|<span data-ttu-id="b4ccd-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4ccd-111">Type</span></span>|<span data-ttu-id="b4ccd-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4ccd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4ccd-113">actionName</span><span class="sxs-lookup"><span data-stu-id="b4ccd-113">actionName</span></span>|<span data-ttu-id="b4ccd-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b4ccd-114">String</span></span>|<span data-ttu-id="b4ccd-115">Nome da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b4ccd-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b4ccd-116">actionState</span><span class="sxs-lookup"><span data-stu-id="b4ccd-116">actionState</span></span>|[<span data-ttu-id="b4ccd-117">actionState</span><span class="sxs-lookup"><span data-stu-id="b4ccd-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="b4ccd-118">Estado da ação Inherited de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="b4ccd-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="b4ccd-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="b4ccd-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="b4ccd-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b4ccd-120">startDateTime</span></span>|<span data-ttu-id="b4ccd-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4ccd-121">DateTimeOffset</span></span>|<span data-ttu-id="b4ccd-122">Hora em que ação foi iniciada, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b4ccd-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b4ccd-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b4ccd-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="b4ccd-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4ccd-124">DateTimeOffset</span></span>|<span data-ttu-id="b4ccd-125">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b4ccd-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b4ccd-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b4ccd-126">userPrincipalName</span></span>|<span data-ttu-id="b4ccd-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b4ccd-127">String</span></span>|<span data-ttu-id="b4ccd-128">Nome da entidade de segurança do usuário a ser excluído</span><span class="sxs-lookup"><span data-stu-id="b4ccd-128">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4ccd-129">Relações</span><span class="sxs-lookup"><span data-stu-id="b4ccd-129">Relationships</span></span>
<span data-ttu-id="b4ccd-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b4ccd-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b4ccd-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b4ccd-131">JSON Representation</span></span>
<span data-ttu-id="b4ccd-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b4ccd-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deleteUserFromSharedAppleDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deleteUserFromSharedAppleDeviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```





