---
title: Tipo de recurso windows10NetworkProxyServer
description: Política de Servidor Proxy de Rede.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4e9f727916f055fe197f98b07625b00406e16e83
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921098"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="846a5-103">Tipo de recurso windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="846a5-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="846a5-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="846a5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="846a5-105">Política de Servidor Proxy de Rede.</span><span class="sxs-lookup"><span data-stu-id="846a5-105">Network Proxy Server Policy.</span></span>
## <a name="properties"></a><span data-ttu-id="846a5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="846a5-106">Properties</span></span>
|<span data-ttu-id="846a5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="846a5-107">Property</span></span>|<span data-ttu-id="846a5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="846a5-108">Type</span></span>|<span data-ttu-id="846a5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="846a5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="846a5-110">address</span><span class="sxs-lookup"><span data-stu-id="846a5-110">address</span></span>|<span data-ttu-id="846a5-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="846a5-111">String</span></span>|<span data-ttu-id="846a5-112">Endereço para o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="846a5-112">Address to the proxy server.</span></span> <span data-ttu-id="846a5-113">Especifique um endereço no formato <server>\[“:”<port>\]</span><span class="sxs-lookup"><span data-stu-id="846a5-113">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="846a5-114">exceptions</span><span class="sxs-lookup"><span data-stu-id="846a5-114">exceptions</span></span>|<span data-ttu-id="846a5-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="846a5-115">String collection</span></span>|<span data-ttu-id="846a5-116">Endereços que não devem usar o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="846a5-116">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="846a5-117">O sistema não usará o servidor proxy para endereços que começam com o conteúdo especificado nesse nó.</span><span class="sxs-lookup"><span data-stu-id="846a5-117">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="846a5-118">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="846a5-118">useForLocalAddresses</span></span>|<span data-ttu-id="846a5-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="846a5-119">Boolean</span></span>|<span data-ttu-id="846a5-120">Especifica se o servidor proxy deve ser usado para endereços locais (intranet).</span><span class="sxs-lookup"><span data-stu-id="846a5-120">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="846a5-121">Relações</span><span class="sxs-lookup"><span data-stu-id="846a5-121">Relationships</span></span>
<span data-ttu-id="846a5-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="846a5-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="846a5-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="846a5-123">JSON Representation</span></span>
<span data-ttu-id="846a5-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="846a5-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10NetworkProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10NetworkProxyServer",
  "address": "String",
  "exceptions": [
    "String"
  ],
  "useForLocalAddresses": true
}
```



