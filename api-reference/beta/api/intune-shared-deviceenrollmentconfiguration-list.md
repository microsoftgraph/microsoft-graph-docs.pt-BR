---
title: Listar deviceEnrollmentConfigurations
description: Listar propriedades e relações de objetos de deviceEnrollmentConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a48df5bd802543a309da4c6a246d4eaadfea57f1
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864176"
---
# <a name="list-deviceenrollmentconfigurations"></a><span data-ttu-id="d8ce1-103">Listar deviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="d8ce1-103">List deviceEnrollmentConfigurations</span></span>

<span data-ttu-id="d8ce1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8ce1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8ce1-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d8ce1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8ce1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d8ce1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8ce1-107">Listar propriedades e relações de objetos de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8ce1-107">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8ce1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d8ce1-108">Prerequisites</span></span>
<span data-ttu-id="d8ce1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8ce1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8ce1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8ce1-111">Permission type</span></span>|<span data-ttu-id="d8ce1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d8ce1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8ce1-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8ce1-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d8ce1-114">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="d8ce1-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="d8ce1-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8ce1-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="d8ce1-116">&nbsp;&nbsp; **Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="d8ce1-116">&nbsp; &nbsp; **Policy Set**</span></span>| <span data-ttu-id="d8ce1-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8ce1-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="d8ce1-118">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8ce1-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8ce1-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8ce1-119">Not supported.</span></span>|
|<span data-ttu-id="d8ce1-120">Application</span><span class="sxs-lookup"><span data-stu-id="d8ce1-120">Application</span></span>||
| <span data-ttu-id="d8ce1-121">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="d8ce1-121">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="d8ce1-122">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8ce1-122">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="d8ce1-123">&nbsp;&nbsp; **Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="d8ce1-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="d8ce1-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8ce1-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8ce1-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8ce1-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d8ce1-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8ce1-126">Request headers</span></span>
|<span data-ttu-id="d8ce1-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d8ce1-127">Header</span></span>|<span data-ttu-id="d8ce1-128">Valor</span><span class="sxs-lookup"><span data-stu-id="d8ce1-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8ce1-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8ce1-129">Authorization</span></span>|<span data-ttu-id="d8ce1-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8ce1-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8ce1-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d8ce1-131">Accept</span></span>|<span data-ttu-id="d8ce1-132">application/json</span><span class="sxs-lookup"><span data-stu-id="d8ce1-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8ce1-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8ce1-133">Request body</span></span>
<span data-ttu-id="d8ce1-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d8ce1-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8ce1-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8ce1-135">Response</span></span>
<span data-ttu-id="d8ce1-136">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8ce1-136">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8ce1-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8ce1-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8ce1-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8ce1-138">Request</span></span>
<span data-ttu-id="d8ce1-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8ce1-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="d8ce1-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8ce1-140">Response</span></span>
<span data-ttu-id="d8ce1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d8ce1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 422

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
      "id": "df13d8b9-d8b9-df13-b9d8-13dfb9d813df",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7
    }
  ]
}
```







