---
title: tipo de recurso de deviceManagementUserRightsSetting
description: Representa uma definição de direitos de usuário.
author: tfitzmac
ms.openlocfilehash: c58a1d3e9a352561a1abec87fa4efa90c599fd7a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313696"
---
# <a name="devicemanagementuserrightssetting-resource-type"></a><span data-ttu-id="81a55-103">tipo de recurso de deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="81a55-103">deviceManagementUserRightsSetting resource type</span></span>

> <span data-ttu-id="81a55-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="81a55-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81a55-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="81a55-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="81a55-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="81a55-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81a55-107">Representa uma definição de direitos de usuário.</span><span class="sxs-lookup"><span data-stu-id="81a55-107">Represents a user rights setting.</span></span>
## <a name="properties"></a><span data-ttu-id="81a55-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="81a55-108">Properties</span></span>
|<span data-ttu-id="81a55-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81a55-109">Property</span></span>|<span data-ttu-id="81a55-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="81a55-110">Type</span></span>|<span data-ttu-id="81a55-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="81a55-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81a55-112">state</span><span class="sxs-lookup"><span data-stu-id="81a55-112">state</span></span>|[<span data-ttu-id="81a55-113">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="81a55-113">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="81a55-114">Configuração de direitos que representa o estado atual deste usuário.</span><span class="sxs-lookup"><span data-stu-id="81a55-114">Representing the current state of this user rights setting.</span></span> <span data-ttu-id="81a55-115">Os valores possíveis são: `notConfigured`, `blocked`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="81a55-115">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="81a55-116">localUsersOrGroups</span><span class="sxs-lookup"><span data-stu-id="81a55-116">localUsersOrGroups</span></span>|<span data-ttu-id="81a55-117">coleção [deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="81a55-117">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) collection</span></span>|<span data-ttu-id="81a55-118">Que representa uma coleção de usuários ou grupos que serão definidos no dispositivo se o estado dessa configuração é permitido locais.</span><span class="sxs-lookup"><span data-stu-id="81a55-118">Representing a collection of local users or groups which will be set on device if the state of this setting is Allowed.</span></span> <span data-ttu-id="81a55-119">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="81a55-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81a55-120">Relações</span><span class="sxs-lookup"><span data-stu-id="81a55-120">Relationships</span></span>
<span data-ttu-id="81a55-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="81a55-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="81a55-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="81a55-122">JSON Representation</span></span>
<span data-ttu-id="81a55-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="81a55-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsSetting",
  "state": "String",
  "localUsersOrGroups": [
    {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
      "name": "String",
      "description": "String",
      "securityIdentifier": "String"
    }
  ]
}
```





