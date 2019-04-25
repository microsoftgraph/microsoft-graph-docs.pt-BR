---
title: Get reportRoot
description: Ler propriedades e relações do objeto reportRoot.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ecfdc13e5e4cdfea5a8c3c9cfb40fe9d6872bd92
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526941"
---
# <a name="get-reportroot"></a><span data-ttu-id="d8eac-103">Get reportRoot</span><span class="sxs-lookup"><span data-stu-id="d8eac-103">Get reportRoot</span></span>

> <span data-ttu-id="d8eac-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d8eac-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d8eac-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d8eac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d8eac-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d8eac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8eac-107">Ler propriedades e relações do objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="d8eac-107">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d8eac-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d8eac-108">Prerequisites</span></span>
<span data-ttu-id="d8eac-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8eac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8eac-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8eac-111">Permission type</span></span>|<span data-ttu-id="d8eac-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d8eac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8eac-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8eac-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d8eac-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="d8eac-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d8eac-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8eac-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="d8eac-116">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="d8eac-116">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="d8eac-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8eac-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d8eac-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8eac-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8eac-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8eac-119">Not supported.</span></span>|
|<span data-ttu-id="d8eac-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8eac-120">Application</span></span>|<span data-ttu-id="d8eac-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8eac-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8eac-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8eac-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d8eac-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d8eac-123">Optional query parameters</span></span>
<span data-ttu-id="d8eac-124">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d8eac-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d8eac-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8eac-125">Request headers</span></span>
|<span data-ttu-id="d8eac-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d8eac-126">Header</span></span>|<span data-ttu-id="d8eac-127">Valor</span><span class="sxs-lookup"><span data-stu-id="d8eac-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8eac-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8eac-128">Authorization</span></span>|<span data-ttu-id="d8eac-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8eac-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8eac-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d8eac-130">Accept</span></span>|<span data-ttu-id="d8eac-131">application/json</span><span class="sxs-lookup"><span data-stu-id="d8eac-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8eac-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8eac-132">Request body</span></span>
<span data-ttu-id="d8eac-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d8eac-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8eac-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8eac-134">Response</span></span>
<span data-ttu-id="d8eac-135">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [reportRoot](../resources/intune-shared-reportroot.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8eac-135">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8eac-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8eac-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="d8eac-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8eac-137">Request</span></span>
<span data-ttu-id="d8eac-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8eac-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports
```

### <a name="response"></a><span data-ttu-id="d8eac-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8eac-139">Response</span></span>
<span data-ttu-id="d8eac-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d8eac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



