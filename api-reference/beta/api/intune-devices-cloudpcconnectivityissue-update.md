---
title: Atualizar cloudPCConnectivityIssue
description: Atualize as propriedades de um objeto cloudPCConnectivityIssue.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d94f7c2409bb4a0a2b09dab066d25c54f8319b87
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665671"
---
# <a name="update-cloudpcconnectivityissue"></a><span data-ttu-id="9588f-103">Atualizar cloudPCConnectivityIssue</span><span class="sxs-lookup"><span data-stu-id="9588f-103">Update cloudPCConnectivityIssue</span></span>

<span data-ttu-id="9588f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9588f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9588f-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9588f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9588f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9588f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9588f-107">Atualize as propriedades de [um objeto cloudPCConnectivityIssue.](../resources/intune-devices-cloudpcconnectivityissue.md)</span><span class="sxs-lookup"><span data-stu-id="9588f-107">Update the properties of a [cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9588f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9588f-108">Prerequisites</span></span>
<span data-ttu-id="9588f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9588f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9588f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9588f-111">Permission type</span></span>|<span data-ttu-id="9588f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9588f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9588f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9588f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9588f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9588f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9588f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9588f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9588f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9588f-116">Not supported.</span></span>|
|<span data-ttu-id="9588f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9588f-117">Application</span></span>|<span data-ttu-id="9588f-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9588f-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9588f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9588f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/cloudPCConnectivityIssues/{cloudPCConnectivityIssueId}
```

## <a name="request-headers"></a><span data-ttu-id="9588f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9588f-120">Request headers</span></span>
|<span data-ttu-id="9588f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9588f-121">Header</span></span>|<span data-ttu-id="9588f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9588f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9588f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9588f-123">Authorization</span></span>|<span data-ttu-id="9588f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9588f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9588f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9588f-125">Accept</span></span>|<span data-ttu-id="9588f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9588f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9588f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9588f-127">Request body</span></span>
<span data-ttu-id="9588f-128">No corpo da solicitação, fornece uma representação JSON para o [objeto cloudPCConnectivityIssue.](../resources/intune-devices-cloudpcconnectivityissue.md)</span><span class="sxs-lookup"><span data-stu-id="9588f-128">In the request body, supply a JSON representation for the [cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md) object.</span></span>

<span data-ttu-id="9588f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md).</span><span class="sxs-lookup"><span data-stu-id="9588f-129">The following table shows the properties that are required when you create the [cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md).</span></span>

|<span data-ttu-id="9588f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9588f-130">Property</span></span>|<span data-ttu-id="9588f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9588f-131">Type</span></span>|<span data-ttu-id="9588f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9588f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9588f-133">id</span><span class="sxs-lookup"><span data-stu-id="9588f-133">id</span></span>|<span data-ttu-id="9588f-134">String</span><span class="sxs-lookup"><span data-stu-id="9588f-134">String</span></span>|<span data-ttu-id="9588f-135">O identificador exclusivo da entidade de evento de problema de conectividade de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9588f-135">The unique identifier of the user experience analytics connectivity issue event entity.</span></span>|
|<span data-ttu-id="9588f-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="9588f-136">deviceId</span></span>|<span data-ttu-id="9588f-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9588f-137">String</span></span>|<span data-ttu-id="9588f-138">O DeviceId do Intune do dispositivo ao que a conexão está associada.</span><span class="sxs-lookup"><span data-stu-id="9588f-138">The Intune DeviceId of the device the connection is associated with.</span></span>|
|<span data-ttu-id="9588f-139">errorCode</span><span class="sxs-lookup"><span data-stu-id="9588f-139">errorCode</span></span>|<span data-ttu-id="9588f-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9588f-140">String</span></span>|<span data-ttu-id="9588f-141">O código de erro do problema de conectividade.</span><span class="sxs-lookup"><span data-stu-id="9588f-141">The error code of the connectivity issue.</span></span>|
|<span data-ttu-id="9588f-142">errorDateTime</span><span class="sxs-lookup"><span data-stu-id="9588f-142">errorDateTime</span></span>|<span data-ttu-id="9588f-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9588f-143">DateTimeOffset</span></span>|<span data-ttu-id="9588f-144">A hora em que a conexão foi iniciada.</span><span class="sxs-lookup"><span data-stu-id="9588f-144">The time that the connection initiated.</span></span> <span data-ttu-id="9588f-145">O tempo é mostrado no formato ISO 8601 e hora UTC (Tempo Universal Coordenado).</span><span class="sxs-lookup"><span data-stu-id="9588f-145">The time is shown in ISO 8601 format and Coordinated Universal Time (UTC) time.</span></span>|
|<span data-ttu-id="9588f-146">userId</span><span class="sxs-lookup"><span data-stu-id="9588f-146">userId</span></span>|<span data-ttu-id="9588f-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9588f-147">String</span></span>|<span data-ttu-id="9588f-148">A ID exclusiva do usuário que inicializa a conexão.</span><span class="sxs-lookup"><span data-stu-id="9588f-148">The unique id of user who initialize the connection.</span></span>|
|<span data-ttu-id="9588f-149">errorDescription</span><span class="sxs-lookup"><span data-stu-id="9588f-149">errorDescription</span></span>|<span data-ttu-id="9588f-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9588f-150">String</span></span>|<span data-ttu-id="9588f-151">A descrição detalhada do que deu errado.</span><span class="sxs-lookup"><span data-stu-id="9588f-151">The detailed description of what went wrong.</span></span>|
|<span data-ttu-id="9588f-152">recommendedAction</span><span class="sxs-lookup"><span data-stu-id="9588f-152">recommendedAction</span></span>|<span data-ttu-id="9588f-153">String</span><span class="sxs-lookup"><span data-stu-id="9588f-153">String</span></span>|<span data-ttu-id="9588f-154">A ação recomendada para corrigir o erro correspondente.</span><span class="sxs-lookup"><span data-stu-id="9588f-154">The recommended action to fix the corresponding error.</span></span>|



## <a name="response"></a><span data-ttu-id="9588f-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="9588f-155">Response</span></span>
<span data-ttu-id="9588f-156">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9588f-156">If successful, this method returns a `200 OK` response code and an updated [cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9588f-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9588f-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="9588f-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9588f-158">Request</span></span>
<span data-ttu-id="9588f-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9588f-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/cloudPCConnectivityIssues/{cloudPCConnectivityIssueId}
Content-type: application/json
Content-length: 325

{
  "@odata.type": "#microsoft.graph.cloudPCConnectivityIssue",
  "deviceId": "Device Id value",
  "errorCode": "Error Code value",
  "errorDateTime": "2016-12-31T23:58:20.6032957-08:00",
  "userId": "User Id value",
  "errorDescription": "Error Description value",
  "recommendedAction": "Recommended Action value"
}
```

### <a name="response"></a><span data-ttu-id="9588f-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="9588f-160">Response</span></span>
<span data-ttu-id="9588f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9588f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 374

{
  "@odata.type": "#microsoft.graph.cloudPCConnectivityIssue",
  "id": "e8e2bf5f-bf5f-e8e2-5fbf-e2e85fbfe2e8",
  "deviceId": "Device Id value",
  "errorCode": "Error Code value",
  "errorDateTime": "2016-12-31T23:58:20.6032957-08:00",
  "userId": "User Id value",
  "errorDescription": "Error Description value",
  "recommendedAction": "Recommended Action value"
}
```




