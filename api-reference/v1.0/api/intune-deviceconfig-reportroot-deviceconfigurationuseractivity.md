---
title: Função deviceConfigurationUserActivity
description: Metadados para o relatório de atividades do usuário de configuração do dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 61e346a1759c643965e24bff62da62974b1adc2c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760734"
---
# <a name="deviceconfigurationuseractivity-function"></a><span data-ttu-id="12af8-103">Função deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="12af8-103">deviceConfigurationUserActivity function</span></span>

<span data-ttu-id="12af8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12af8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12af8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="12af8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12af8-106">Metadados para o relatório de atividades do usuário de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="12af8-106">Metadata for the device configuration user activity report</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12af8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="12af8-107">Prerequisites</span></span>
<span data-ttu-id="12af8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12af8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12af8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12af8-110">Permission type</span></span>|<span data-ttu-id="12af8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="12af8-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12af8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12af8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="12af8-113">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="12af8-113">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="12af8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12af8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12af8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12af8-115">Not supported.</span></span>|
|<span data-ttu-id="12af8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12af8-116">Application</span></span>|<span data-ttu-id="12af8-117">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="12af8-117">DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12af8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12af8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationUserActivity
```

## <a name="request-headers"></a><span data-ttu-id="12af8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12af8-119">Request headers</span></span>
|<span data-ttu-id="12af8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="12af8-120">Header</span></span>|<span data-ttu-id="12af8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="12af8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12af8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="12af8-122">Authorization</span></span>|<span data-ttu-id="12af8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12af8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12af8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="12af8-124">Accept</span></span>|<span data-ttu-id="12af8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="12af8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12af8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12af8-126">Request body</span></span>
<span data-ttu-id="12af8-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="12af8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12af8-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="12af8-128">Response</span></span>
<span data-ttu-id="12af8-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-deviceconfig-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12af8-129">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-deviceconfig-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12af8-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12af8-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="12af8-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12af8-131">Request</span></span>
<span data-ttu-id="12af8-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="12af8-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationUserActivity
```

### <a name="response"></a><span data-ttu-id="12af8-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="12af8-133">Response</span></span>
<span data-ttu-id="12af8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="12af8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 136

{
  "value": {
    "@odata.type": "microsoft.graph.report",
    "content": "Y29udGVudCBJbnR1bmUgRG9jIFNhbXBsZSAxNTYxOTcwNjY1"
  }
}
```




