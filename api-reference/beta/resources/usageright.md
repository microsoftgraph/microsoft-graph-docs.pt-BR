---
title: Tipo de recurso usageRight
description: Contém informações sobre um usageRight que um usuário/dispositivo atribuiu
author: jeeshnair
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 3f54fb6b54f08d28ab63bf2ec70180c5e0daf490
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159815"
---
# <a name="usageright-resource-type"></a><span data-ttu-id="95c45-103">Tipo de recurso usageRight</span><span class="sxs-lookup"><span data-stu-id="95c45-103">usageRight resource type</span></span>

<span data-ttu-id="95c45-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95c45-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95c45-105">Um direito de uso representa uma licença que um usuário ou dispositivo tem para software de terceiros criado em aplicativos de energia ou para assinaturas baseadas em dispositivos (somente dispositivo).</span><span class="sxs-lookup"><span data-stu-id="95c45-105">A usage right represents a license that a user or device has for either third party software built on power apps or for device based subscriptions (device only).</span></span>

## <a name="methods"></a><span data-ttu-id="95c45-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="95c45-106">Methods</span></span>

|<span data-ttu-id="95c45-107">Método</span><span class="sxs-lookup"><span data-stu-id="95c45-107">Method</span></span>|<span data-ttu-id="95c45-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="95c45-108">Return type</span></span>|<span data-ttu-id="95c45-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="95c45-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="95c45-110">Listar usageRights do usuário</span><span class="sxs-lookup"><span data-stu-id="95c45-110">List user usageRights</span></span>](../api/user-list-usagerights.md)|<span data-ttu-id="95c45-111">Coleção [usageRight](../resources/usageright.md)</span><span class="sxs-lookup"><span data-stu-id="95c45-111">[usageRight](../resources/usageright.md) collection</span></span>|<span data-ttu-id="95c45-112">Obter a lista de direitos de uso de um usuário.</span><span class="sxs-lookup"><span data-stu-id="95c45-112">Get the list of usage rights for a user.</span></span>|
|[<span data-ttu-id="95c45-113">Listar usageRights do dispositivo</span><span class="sxs-lookup"><span data-stu-id="95c45-113">List device usageRights</span></span>](../api/device-list-usagerights.md)|<span data-ttu-id="95c45-114">Coleção [usageRight](../resources/usageright.md)</span><span class="sxs-lookup"><span data-stu-id="95c45-114">[usageRight](../resources/usageright.md) collection</span></span>|<span data-ttu-id="95c45-115">Obter a lista de direitos de uso de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="95c45-115">Get the list of usage rights for a device.</span></span>|

## <a name="properties"></a><span data-ttu-id="95c45-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="95c45-116">Properties</span></span>

|<span data-ttu-id="95c45-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="95c45-117">Property</span></span>|<span data-ttu-id="95c45-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="95c45-118">Type</span></span>|<span data-ttu-id="95c45-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="95c45-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95c45-120">catalogId</span><span class="sxs-lookup"><span data-stu-id="95c45-120">catalogId</span></span>|<span data-ttu-id="95c45-121">String</span><span class="sxs-lookup"><span data-stu-id="95c45-121">String</span></span>|<span data-ttu-id="95c45-122">ID do produto correspondente ao direito de uso.</span><span class="sxs-lookup"><span data-stu-id="95c45-122">Product id corresponding to the usage right.</span></span>|
|<span data-ttu-id="95c45-123">id</span><span class="sxs-lookup"><span data-stu-id="95c45-123">id</span></span>|<span data-ttu-id="95c45-124">String</span><span class="sxs-lookup"><span data-stu-id="95c45-124">String</span></span>|<span data-ttu-id="95c45-125">A ID do direito de uso.</span><span class="sxs-lookup"><span data-stu-id="95c45-125">The id of the usage right.</span></span>|
|<span data-ttu-id="95c45-126">serviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="95c45-126">serviceIdentifier</span></span>|<span data-ttu-id="95c45-127">String</span><span class="sxs-lookup"><span data-stu-id="95c45-127">String</span></span>|<span data-ttu-id="95c45-128">Identificador do serviço correspondente ao direito de uso.</span><span class="sxs-lookup"><span data-stu-id="95c45-128">Identifier of the service corresponding to the usage right.</span></span>|
|<span data-ttu-id="95c45-129">estado</span><span class="sxs-lookup"><span data-stu-id="95c45-129">state</span></span>|<span data-ttu-id="95c45-130">usageRightState</span><span class="sxs-lookup"><span data-stu-id="95c45-130">usageRightState</span></span>|<span data-ttu-id="95c45-131">O estado do direito de uso.</span><span class="sxs-lookup"><span data-stu-id="95c45-131">The state of the usage right.</span></span> <span data-ttu-id="95c45-132">Os valores possíveis são: `active`, `inactive`, `warning`, `suspended`.</span><span class="sxs-lookup"><span data-stu-id="95c45-132">Possible values are: `active`, `inactive`, `warning`, `suspended`.</span></span>|

### <a name="usagerightstate-values"></a><span data-ttu-id="95c45-133">Valores usageRightState</span><span class="sxs-lookup"><span data-stu-id="95c45-133">usageRightState values</span></span> 

| <span data-ttu-id="95c45-134">Member</span><span class="sxs-lookup"><span data-stu-id="95c45-134">Member</span></span>             |  <span data-ttu-id="95c45-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="95c45-135">Description</span></span>               |
| :----------------- |  :------------------------ |
|<span data-ttu-id="95c45-136">ativo</span><span class="sxs-lookup"><span data-stu-id="95c45-136">active</span></span>              | <span data-ttu-id="95c45-137">Indica que o direito de uso está ativo e pode ser usado para benefícios de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="95c45-137">Indicates that the usage right is active and can be used for provisioning benefits.</span></span>|
|<span data-ttu-id="95c45-138">inativo</span><span class="sxs-lookup"><span data-stu-id="95c45-138">inactive</span></span>                | <span data-ttu-id="95c45-139">Indica que o direito de uso não está ativo e não pode ser usado para benefícios de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="95c45-139">Indicates that the usage right is not active and cannot be used for provisioning benefits.</span></span>|
|<span data-ttu-id="95c45-140">warning</span><span class="sxs-lookup"><span data-stu-id="95c45-140">warning</span></span>                | <span data-ttu-id="95c45-141">Indica que o direito de uso está em carência provavelmente devido à violação do pagamento.</span><span class="sxs-lookup"><span data-stu-id="95c45-141">Indicates that the usage right is in grace likely due to payment violation.</span></span> <span data-ttu-id="95c45-142">Esse estado pode ser usado para lembrar o pagamento pendente ou oferecer uma experiência degradada.</span><span class="sxs-lookup"><span data-stu-id="95c45-142">This state can be used to either remind of pending payment or offer a degraded experience.</span></span>|
|<span data-ttu-id="95c45-143">suspended</span><span class="sxs-lookup"><span data-stu-id="95c45-143">suspended</span></span>                | <span data-ttu-id="95c45-144">Indica que o direito de uso é suspenso provavelmente devido a violação de pagamento</span><span class="sxs-lookup"><span data-stu-id="95c45-144">Indicates that the usage right is suspended likely due to Payment violation</span></span>|
|<span data-ttu-id="95c45-145">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="95c45-145">unknownFutureValue</span></span>      | <span data-ttu-id="95c45-146">Valor do Sentinel para indicar valores futuros.</span><span class="sxs-lookup"><span data-stu-id="95c45-146">Sentinel value to indicate future values.</span></span> |

><span data-ttu-id="95c45-147">**Observação:** Somente os estados ativos e de aviso representam um benefício que pode ser usável.</span><span class="sxs-lookup"><span data-stu-id="95c45-147">**Note:** Only the active and warning states represent a usable benefit.</span></span> <span data-ttu-id="95c45-148">Todos os outros estados devem ser tratados como não resultando em um benefício usável.</span><span class="sxs-lookup"><span data-stu-id="95c45-148">All other states should be treated as not resulting in a usable benefit.</span></span>



## <a name="relationships"></a><span data-ttu-id="95c45-149">Relações</span><span class="sxs-lookup"><span data-stu-id="95c45-149">Relationships</span></span>

<span data-ttu-id="95c45-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="95c45-150">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="95c45-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="95c45-151">JSON representation</span></span>

<span data-ttu-id="95c45-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="95c45-152">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.usageRight",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.usageRight",
  "id": "String (identifier)",
  "catalogId": "String",
  "serviceIdentifier": "String",
  "state": "String"
}
```

