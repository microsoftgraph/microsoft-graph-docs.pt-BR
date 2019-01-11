---
title: tipo de recurso de deviceManagementUserRightsSetting
description: Representa uma definição de direitos de usuário.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b12dc0c1c682b59ef741b3d49083fd0739d27abb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844804"
---
# <a name="devicemanagementuserrightssetting-resource-type"></a><span data-ttu-id="78c3b-103">tipo de recurso de deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="78c3b-103">deviceManagementUserRightsSetting resource type</span></span>

> <span data-ttu-id="78c3b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="78c3b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78c3b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="78c3b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="78c3b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="78c3b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="78c3b-107">Representa uma definição de direitos de usuário.</span><span class="sxs-lookup"><span data-stu-id="78c3b-107">Represents a user rights setting.</span></span>
## <a name="properties"></a><span data-ttu-id="78c3b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="78c3b-108">Properties</span></span>
|<span data-ttu-id="78c3b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="78c3b-109">Property</span></span>|<span data-ttu-id="78c3b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="78c3b-110">Type</span></span>|<span data-ttu-id="78c3b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="78c3b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78c3b-112">state</span><span class="sxs-lookup"><span data-stu-id="78c3b-112">state</span></span>|[<span data-ttu-id="78c3b-113">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="78c3b-113">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="78c3b-114">Configuração de direitos que representa o estado atual deste usuário.</span><span class="sxs-lookup"><span data-stu-id="78c3b-114">Representing the current state of this user rights setting.</span></span> <span data-ttu-id="78c3b-115">Os valores possíveis são: `notConfigured`, `blocked`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="78c3b-115">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="78c3b-116">localUsersOrGroups</span><span class="sxs-lookup"><span data-stu-id="78c3b-116">localUsersOrGroups</span></span>|<span data-ttu-id="78c3b-117">coleção [deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="78c3b-117">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) collection</span></span>|<span data-ttu-id="78c3b-118">Que representa uma coleção de usuários ou grupos que serão definidos no dispositivo se o estado dessa configuração é permitido locais.</span><span class="sxs-lookup"><span data-stu-id="78c3b-118">Representing a collection of local users or groups which will be set on device if the state of this setting is Allowed.</span></span> <span data-ttu-id="78c3b-119">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="78c3b-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78c3b-120">Relações</span><span class="sxs-lookup"><span data-stu-id="78c3b-120">Relationships</span></span>
<span data-ttu-id="78c3b-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="78c3b-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="78c3b-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="78c3b-122">JSON Representation</span></span>
<span data-ttu-id="78c3b-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="78c3b-123">Here is a JSON representation of the resource.</span></span>
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





