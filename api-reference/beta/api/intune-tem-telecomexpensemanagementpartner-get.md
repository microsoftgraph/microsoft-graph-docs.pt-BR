---
title: Obter telecomExpenseManagementPartner
description: Ler propriedades de leitura e relações do objeto telecomExpenseManagementPartner.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b90452cbf23189cf05dd432c9673d2c95a6990b5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526731"
---
# <a name="get-telecomexpensemanagementpartner"></a><span data-ttu-id="7c8cc-103">Obter telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="7c8cc-103">Get telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="7c8cc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7c8cc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c8cc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7c8cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c8cc-106">Ler propriedades de leitura e relações do objeto [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="7c8cc-106">Read properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c8cc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7c8cc-107">Prerequisites</span></span>
<span data-ttu-id="7c8cc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c8cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c8cc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c8cc-110">Permission type</span></span>|<span data-ttu-id="7c8cc-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7c8cc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c8cc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c8cc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7c8cc-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c8cc-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="7c8cc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c8cc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c8cc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c8cc-115">Not supported.</span></span>|
|<span data-ttu-id="7c8cc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7c8cc-116">Application</span></span>|<span data-ttu-id="7c8cc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c8cc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c8cc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c8cc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7c8cc-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7c8cc-119">Optional query parameters</span></span>
<span data-ttu-id="7c8cc-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7c8cc-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7c8cc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c8cc-121">Request headers</span></span>
|<span data-ttu-id="7c8cc-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7c8cc-122">Header</span></span>|<span data-ttu-id="7c8cc-123">Valor</span><span class="sxs-lookup"><span data-stu-id="7c8cc-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c8cc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c8cc-124">Authorization</span></span>|<span data-ttu-id="7c8cc-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c8cc-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c8cc-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7c8cc-126">Accept</span></span>|<span data-ttu-id="7c8cc-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7c8cc-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c8cc-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7c8cc-128">Request body</span></span>
<span data-ttu-id="7c8cc-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7c8cc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c8cc-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c8cc-130">Response</span></span>
<span data-ttu-id="7c8cc-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c8cc-131">If successful, this method returns a `200 OK` response code and [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c8cc-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7c8cc-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c8cc-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c8cc-133">Request</span></span>
<span data-ttu-id="7c8cc-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c8cc-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="7c8cc-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c8cc-135">Response</span></span>
<span data-ttu-id="7c8cc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7c8cc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 330

{
  "value": {
    "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
    "id": "47a3b399-b399-47a3-99b3-a34799b3a347",
    "displayName": "Display Name value",
    "url": "Url value",
    "appAuthorized": true,
    "enabled": true,
    "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
  }
}
```





