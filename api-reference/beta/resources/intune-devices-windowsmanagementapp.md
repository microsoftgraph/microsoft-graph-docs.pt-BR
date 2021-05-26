---
title: Tipo de recurso windowsManagementApp
description: Windows de aplicativo de gerenciamento.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 540ba41779e64c57b5c74c7acf004172a1567c37
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665571"
---
# <a name="windowsmanagementapp-resource-type"></a><span data-ttu-id="3180d-103">Tipo de recurso windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="3180d-103">windowsManagementApp resource type</span></span>

<span data-ttu-id="3180d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3180d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3180d-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3180d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3180d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3180d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3180d-107">Windows de aplicativo de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="3180d-107">Windows management app entity.</span></span>

## <a name="methods"></a><span data-ttu-id="3180d-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="3180d-108">Methods</span></span>
|<span data-ttu-id="3180d-109">Método</span><span class="sxs-lookup"><span data-stu-id="3180d-109">Method</span></span>|<span data-ttu-id="3180d-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3180d-110">Return Type</span></span>|<span data-ttu-id="3180d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3180d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3180d-112">Obter windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="3180d-112">Get windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-get.md)|[<span data-ttu-id="3180d-113">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="3180d-113">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="3180d-114">Leia propriedades e relações do [objeto windowsManagementApp.](../resources/intune-devices-windowsmanagementapp.md)</span><span class="sxs-lookup"><span data-stu-id="3180d-114">Read properties and relationships of the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|
|[<span data-ttu-id="3180d-115">Atualizar windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="3180d-115">Update windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-update.md)|[<span data-ttu-id="3180d-116">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="3180d-116">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="3180d-117">Atualize as propriedades de um [objeto windowsManagementApp.](../resources/intune-devices-windowsmanagementapp.md)</span><span class="sxs-lookup"><span data-stu-id="3180d-117">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|
|[<span data-ttu-id="3180d-118">ação setAsManagedInstaller</span><span class="sxs-lookup"><span data-stu-id="3180d-118">setAsManagedInstaller action</span></span>](../api/intune-devices-windowsmanagementapp-setasmanagedinstaller.md)|<span data-ttu-id="3180d-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="3180d-119">None</span></span>|<span data-ttu-id="3180d-120">Definir o status do Instalador Gerenciado para o locatário do chamador</span><span class="sxs-lookup"><span data-stu-id="3180d-120">Set the Managed Installer status for the caller tenant</span></span>|

## <a name="properties"></a><span data-ttu-id="3180d-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3180d-121">Properties</span></span>
|<span data-ttu-id="3180d-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3180d-122">Property</span></span>|<span data-ttu-id="3180d-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="3180d-123">Type</span></span>|<span data-ttu-id="3180d-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="3180d-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3180d-125">id</span><span class="sxs-lookup"><span data-stu-id="3180d-125">id</span></span>|<span data-ttu-id="3180d-126">String</span><span class="sxs-lookup"><span data-stu-id="3180d-126">String</span></span>|<span data-ttu-id="3180d-127">Identificador exclusivo do aplicativo Windows de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="3180d-127">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="3180d-128">availableVersion</span><span class="sxs-lookup"><span data-stu-id="3180d-128">availableVersion</span></span>|<span data-ttu-id="3180d-129">String</span><span class="sxs-lookup"><span data-stu-id="3180d-129">String</span></span>|<span data-ttu-id="3180d-130">Windows versão disponível do aplicativo de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="3180d-130">Windows management app available version.</span></span>|
|<span data-ttu-id="3180d-131">managedInstaller</span><span class="sxs-lookup"><span data-stu-id="3180d-131">managedInstaller</span></span>|[<span data-ttu-id="3180d-132">managedInstallerStatus</span><span class="sxs-lookup"><span data-stu-id="3180d-132">managedInstallerStatus</span></span>](../resources/intune-devices-managedinstallerstatus.md)|<span data-ttu-id="3180d-133">Status do Instalador Gerenciado.</span><span class="sxs-lookup"><span data-stu-id="3180d-133">Managed Installer Status.</span></span> <span data-ttu-id="3180d-134">Os valores possíveis são: `disabled` e `enabled`.</span><span class="sxs-lookup"><span data-stu-id="3180d-134">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="3180d-135">managedInstallerConfiguredDateTime</span><span class="sxs-lookup"><span data-stu-id="3180d-135">managedInstallerConfiguredDateTime</span></span>|<span data-ttu-id="3180d-136">String</span><span class="sxs-lookup"><span data-stu-id="3180d-136">String</span></span>|<span data-ttu-id="3180d-137">Data configurada do Instalador Gerenciado</span><span class="sxs-lookup"><span data-stu-id="3180d-137">Managed Installer Configured Date Time</span></span>|

## <a name="relationships"></a><span data-ttu-id="3180d-138">Relações</span><span class="sxs-lookup"><span data-stu-id="3180d-138">Relationships</span></span>
|<span data-ttu-id="3180d-139">Relação</span><span class="sxs-lookup"><span data-stu-id="3180d-139">Relationship</span></span>|<span data-ttu-id="3180d-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="3180d-140">Type</span></span>|<span data-ttu-id="3180d-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="3180d-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3180d-142">healthStates</span><span class="sxs-lookup"><span data-stu-id="3180d-142">healthStates</span></span>|<span data-ttu-id="3180d-143">[coleção windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)</span><span class="sxs-lookup"><span data-stu-id="3180d-143">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) collection</span></span>|<span data-ttu-id="3180d-144">A lista de estados de saúde para o aplicativo de gerenciamento Windows instalado.</span><span class="sxs-lookup"><span data-stu-id="3180d-144">The list of health states for installed Windows management app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3180d-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3180d-145">JSON Representation</span></span>
<span data-ttu-id="3180d-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3180d-146">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "String (identifier)",
  "availableVersion": "String",
  "managedInstaller": "String",
  "managedInstallerConfiguredDateTime": "String"
}
```




