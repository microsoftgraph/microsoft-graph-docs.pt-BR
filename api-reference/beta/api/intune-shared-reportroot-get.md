---
title: Get reportRoot
description: Ler propriedades e relações do objeto reportRoot.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 73eec43bbaf31d39e99cdad5e859debc08b08558
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2019
ms.locfileid: "30570931"
---
# <a name="get-reportroot"></a><span data-ttu-id="c9b9a-103">Get reportRoot</span><span class="sxs-lookup"><span data-stu-id="c9b9a-103">Get reportRoot</span></span>

> <span data-ttu-id="c9b9a-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c9b9a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c9b9a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c9b9a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c9b9a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c9b9a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9b9a-107">Ler propriedades e relações do objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="c9b9a-107">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c9b9a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c9b9a-108">Prerequisites</span></span>
<span data-ttu-id="c9b9a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c9b9a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c9b9a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c9b9a-111">Permission type</span></span>|<span data-ttu-id="c9b9a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c9b9a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9b9a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c9b9a-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c9b9a-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="c9b9a-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="c9b9a-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c9b9a-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="c9b9a-116">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="c9b9a-116">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="c9b9a-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c9b9a-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="c9b9a-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c9b9a-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9b9a-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9b9a-119">Not supported.</span></span>|
|<span data-ttu-id="c9b9a-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c9b9a-120">Application</span></span>|<span data-ttu-id="c9b9a-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9b9a-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9b9a-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9b9a-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c9b9a-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c9b9a-123">Optional query parameters</span></span>
<span data-ttu-id="c9b9a-124">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c9b9a-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c9b9a-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c9b9a-125">Request headers</span></span>
|<span data-ttu-id="c9b9a-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c9b9a-126">Header</span></span>|<span data-ttu-id="c9b9a-127">Valor</span><span class="sxs-lookup"><span data-stu-id="c9b9a-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9b9a-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9b9a-128">Authorization</span></span>|<span data-ttu-id="c9b9a-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9b9a-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9b9a-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c9b9a-130">Accept</span></span>|<span data-ttu-id="c9b9a-131">application/json</span><span class="sxs-lookup"><span data-stu-id="c9b9a-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9b9a-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9b9a-132">Request body</span></span>
<span data-ttu-id="c9b9a-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c9b9a-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9b9a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9b9a-134">Response</span></span>
<span data-ttu-id="c9b9a-135">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [reportRoot](../resources/intune-shared-reportroot.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c9b9a-135">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9b9a-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c9b9a-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="c9b9a-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9b9a-137">Request</span></span>
<span data-ttu-id="c9b9a-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c9b9a-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports
```

### <a name="response"></a><span data-ttu-id="c9b9a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9b9a-139">Response</span></span>
<span data-ttu-id="c9b9a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c9b9a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 124

{
  "value": {
    "@odata.type": "#microsoft.graph.reportRoot",
    "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
  }
}
```



