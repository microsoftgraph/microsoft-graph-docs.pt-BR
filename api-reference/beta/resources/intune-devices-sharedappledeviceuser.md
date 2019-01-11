---
title: tipo de recurso de sharedAppleDeviceUser
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5ee74080b95328cf55813dc628ee7a517dff08e8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806850"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="46bd0-103">tipo de recurso de sharedAppleDeviceUser</span><span class="sxs-lookup"><span data-stu-id="46bd0-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="46bd0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="46bd0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46bd0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="46bd0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="46bd0-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="46bd0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="46bd0-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="46bd0-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="46bd0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="46bd0-108">Properties</span></span>
|<span data-ttu-id="46bd0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46bd0-109">Property</span></span>|<span data-ttu-id="46bd0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="46bd0-110">Type</span></span>|<span data-ttu-id="46bd0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="46bd0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46bd0-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="46bd0-112">userPrincipalName</span></span>|<span data-ttu-id="46bd0-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="46bd0-113">String</span></span>|<span data-ttu-id="46bd0-114">Nome de usuário</span><span class="sxs-lookup"><span data-stu-id="46bd0-114">User name</span></span>|
|<span data-ttu-id="46bd0-115">dataToSync</span><span class="sxs-lookup"><span data-stu-id="46bd0-115">dataToSync</span></span>|<span data-ttu-id="46bd0-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="46bd0-116">Boolean</span></span>|<span data-ttu-id="46bd0-117">Dados a serem sincronizados</span><span class="sxs-lookup"><span data-stu-id="46bd0-117">Data to sync</span></span>|
|<span data-ttu-id="46bd0-118">dataQuota</span><span class="sxs-lookup"><span data-stu-id="46bd0-118">dataQuota</span></span>|<span data-ttu-id="46bd0-119">Int64</span><span class="sxs-lookup"><span data-stu-id="46bd0-119">Int64</span></span>|<span data-ttu-id="46bd0-120">Cota de dados</span><span class="sxs-lookup"><span data-stu-id="46bd0-120">Data quota</span></span>|
|<span data-ttu-id="46bd0-121">dataUsed</span><span class="sxs-lookup"><span data-stu-id="46bd0-121">dataUsed</span></span>|<span data-ttu-id="46bd0-122">Int64</span><span class="sxs-lookup"><span data-stu-id="46bd0-122">Int64</span></span>|<span data-ttu-id="46bd0-123">Cota de dados</span><span class="sxs-lookup"><span data-stu-id="46bd0-123">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="46bd0-124">Relações</span><span class="sxs-lookup"><span data-stu-id="46bd0-124">Relationships</span></span>
<span data-ttu-id="46bd0-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="46bd0-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="46bd0-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="46bd0-126">JSON Representation</span></span>
<span data-ttu-id="46bd0-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="46bd0-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharedAppleDeviceUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedAppleDeviceUser",
  "userPrincipalName": "String",
  "dataToSync": true,
  "dataQuota": 1024,
  "dataUsed": 1024
}
```





