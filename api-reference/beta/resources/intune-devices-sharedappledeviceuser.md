---
title: tipo de recurso de sharedAppleDeviceUser
description: Ainda não documentado
ms.openlocfilehash: 79ebc5ae520c1c9b40bffb6a86e95693c52fa1e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035095"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="42a96-103">tipo de recurso de sharedAppleDeviceUser</span><span class="sxs-lookup"><span data-stu-id="42a96-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="42a96-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="42a96-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42a96-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="42a96-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="42a96-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="42a96-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="42a96-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="42a96-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="42a96-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="42a96-108">Properties</span></span>
|<span data-ttu-id="42a96-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42a96-109">Property</span></span>|<span data-ttu-id="42a96-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="42a96-110">Type</span></span>|<span data-ttu-id="42a96-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="42a96-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42a96-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="42a96-112">userPrincipalName</span></span>|<span data-ttu-id="42a96-113">String</span><span class="sxs-lookup"><span data-stu-id="42a96-113">String</span></span>|<span data-ttu-id="42a96-114">Nome de usuário</span><span class="sxs-lookup"><span data-stu-id="42a96-114">User name</span></span>|
|<span data-ttu-id="42a96-115">dataToSync</span><span class="sxs-lookup"><span data-stu-id="42a96-115">dataToSync</span></span>|<span data-ttu-id="42a96-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="42a96-116">Boolean</span></span>|<span data-ttu-id="42a96-117">Dados a serem sincronizados</span><span class="sxs-lookup"><span data-stu-id="42a96-117">Data to sync</span></span>|
|<span data-ttu-id="42a96-118">dataQuota</span><span class="sxs-lookup"><span data-stu-id="42a96-118">dataQuota</span></span>|<span data-ttu-id="42a96-119">Int64</span><span class="sxs-lookup"><span data-stu-id="42a96-119">Int64</span></span>|<span data-ttu-id="42a96-120">Cota de dados</span><span class="sxs-lookup"><span data-stu-id="42a96-120">Data quota</span></span>|
|<span data-ttu-id="42a96-121">dataUsed</span><span class="sxs-lookup"><span data-stu-id="42a96-121">dataUsed</span></span>|<span data-ttu-id="42a96-122">Int64</span><span class="sxs-lookup"><span data-stu-id="42a96-122">Int64</span></span>|<span data-ttu-id="42a96-123">Cota de dados</span><span class="sxs-lookup"><span data-stu-id="42a96-123">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="42a96-124">Relações</span><span class="sxs-lookup"><span data-stu-id="42a96-124">Relationships</span></span>
<span data-ttu-id="42a96-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="42a96-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="42a96-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="42a96-126">JSON Representation</span></span>
<span data-ttu-id="42a96-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="42a96-127">Here is a JSON representation of the resource.</span></span>
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





