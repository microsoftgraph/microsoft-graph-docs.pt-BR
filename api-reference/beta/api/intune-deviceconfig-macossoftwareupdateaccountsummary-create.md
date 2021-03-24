---
title: Criar macOSSoftwareUpdateAccountSummary
description: Crie um novo objeto macOSSoftwareUpdateAccountSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0a34b35952ee240784a4b4f28705fe49354024cb
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129752"
---
# <a name="create-macossoftwareupdateaccountsummary"></a><span data-ttu-id="376f1-103">Criar macOSSoftwareUpdateAccountSummary</span><span class="sxs-lookup"><span data-stu-id="376f1-103">Create macOSSoftwareUpdateAccountSummary</span></span>

<span data-ttu-id="376f1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="376f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="376f1-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="376f1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="376f1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="376f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="376f1-107">Crie um novo [objeto macOSSoftwareUpdateAccountSummary.](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)</span><span class="sxs-lookup"><span data-stu-id="376f1-107">Create a new [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="376f1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="376f1-108">Prerequisites</span></span>
<span data-ttu-id="376f1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="376f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="376f1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="376f1-111">Permission type</span></span>|<span data-ttu-id="376f1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="376f1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="376f1-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="376f1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="376f1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="376f1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="376f1-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="376f1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="376f1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="376f1-116">Not supported.</span></span>|
|<span data-ttu-id="376f1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="376f1-117">Application</span></span>|<span data-ttu-id="376f1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="376f1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="376f1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="376f1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/macOSSoftwareUpdateAccountSummaries
```

## <a name="request-headers"></a><span data-ttu-id="376f1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="376f1-120">Request headers</span></span>
|<span data-ttu-id="376f1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="376f1-121">Header</span></span>|<span data-ttu-id="376f1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="376f1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="376f1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="376f1-123">Authorization</span></span>|<span data-ttu-id="376f1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="376f1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="376f1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="376f1-125">Accept</span></span>|<span data-ttu-id="376f1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="376f1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="376f1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="376f1-127">Request body</span></span>
<span data-ttu-id="376f1-128">No corpo da solicitação, fornece uma representação JSON para o objeto macOSSoftwareUpdateAccountSummary.</span><span class="sxs-lookup"><span data-stu-id="376f1-128">In the request body, supply a JSON representation for the macOSSoftwareUpdateAccountSummary object.</span></span>

<span data-ttu-id="376f1-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o macOSSoftwareUpdateAccountSummary.</span><span class="sxs-lookup"><span data-stu-id="376f1-129">The following table shows the properties that are required when you create the macOSSoftwareUpdateAccountSummary.</span></span>

|<span data-ttu-id="376f1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="376f1-130">Property</span></span>|<span data-ttu-id="376f1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="376f1-131">Type</span></span>|<span data-ttu-id="376f1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="376f1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="376f1-133">id</span><span class="sxs-lookup"><span data-stu-id="376f1-133">id</span></span>|<span data-ttu-id="376f1-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="376f1-134">String</span></span>|<span data-ttu-id="376f1-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="376f1-135">Key of the entity.</span></span>|
|<span data-ttu-id="376f1-136">displayName</span><span class="sxs-lookup"><span data-stu-id="376f1-136">displayName</span></span>|<span data-ttu-id="376f1-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="376f1-137">String</span></span>|<span data-ttu-id="376f1-138">O nome do relatório</span><span class="sxs-lookup"><span data-stu-id="376f1-138">The name of the report</span></span>|
|<span data-ttu-id="376f1-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="376f1-139">deviceId</span></span>|<span data-ttu-id="376f1-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="376f1-140">String</span></span>|<span data-ttu-id="376f1-141">A ID do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="376f1-141">The device ID.</span></span>|
|<span data-ttu-id="376f1-142">userId</span><span class="sxs-lookup"><span data-stu-id="376f1-142">userId</span></span>|<span data-ttu-id="376f1-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="376f1-143">String</span></span>|<span data-ttu-id="376f1-144">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="376f1-144">The user ID.</span></span>|
|<span data-ttu-id="376f1-145">deviceName</span><span class="sxs-lookup"><span data-stu-id="376f1-145">deviceName</span></span>|<span data-ttu-id="376f1-146">String</span><span class="sxs-lookup"><span data-stu-id="376f1-146">String</span></span>|<span data-ttu-id="376f1-147">O nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="376f1-147">The device name.</span></span>|
|<span data-ttu-id="376f1-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="376f1-148">userPrincipalName</span></span>|<span data-ttu-id="376f1-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="376f1-149">String</span></span>|<span data-ttu-id="376f1-150">O nome principal do usuário</span><span class="sxs-lookup"><span data-stu-id="376f1-150">The user principal name</span></span>|
|<span data-ttu-id="376f1-151">osVersion</span><span class="sxs-lookup"><span data-stu-id="376f1-151">osVersion</span></span>|<span data-ttu-id="376f1-152">String</span><span class="sxs-lookup"><span data-stu-id="376f1-152">String</span></span>|<span data-ttu-id="376f1-153">A versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="376f1-153">The OS version.</span></span>|
|<span data-ttu-id="376f1-154">successfulUpdateCount</span><span class="sxs-lookup"><span data-stu-id="376f1-154">successfulUpdateCount</span></span>|<span data-ttu-id="376f1-155">Int32</span><span class="sxs-lookup"><span data-stu-id="376f1-155">Int32</span></span>|<span data-ttu-id="376f1-156">Número de atualizações bem-sucedidas no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="376f1-156">Number of successful updates on the device.</span></span>|
|<span data-ttu-id="376f1-157">failedUpdateCount</span><span class="sxs-lookup"><span data-stu-id="376f1-157">failedUpdateCount</span></span>|<span data-ttu-id="376f1-158">Int32</span><span class="sxs-lookup"><span data-stu-id="376f1-158">Int32</span></span>|<span data-ttu-id="376f1-159">Número de atualizações com falha no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="376f1-159">Number of failed updates on the device.</span></span>|
|<span data-ttu-id="376f1-160">totalUpdateCount</span><span class="sxs-lookup"><span data-stu-id="376f1-160">totalUpdateCount</span></span>|<span data-ttu-id="376f1-161">Int32</span><span class="sxs-lookup"><span data-stu-id="376f1-161">Int32</span></span>|<span data-ttu-id="376f1-162">Número de atualizações totais no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="376f1-162">Number of total updates on the device.</span></span>|
|<span data-ttu-id="376f1-163">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="376f1-163">lastUpdatedDateTime</span></span>|<span data-ttu-id="376f1-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="376f1-164">DateTimeOffset</span></span>|<span data-ttu-id="376f1-165">Última data em que o relatório deste dispositivo foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="376f1-165">Last date time the report for this device was updated.</span></span>|



## <a name="response"></a><span data-ttu-id="376f1-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="376f1-166">Response</span></span>
<span data-ttu-id="376f1-167">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="376f1-167">If successful, this method returns a `201 Created` response code and a [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="376f1-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="376f1-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="376f1-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="376f1-169">Request</span></span>
<span data-ttu-id="376f1-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="376f1-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/macOSSoftwareUpdateAccountSummaries
Content-type: application/json
Content-length: 453

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateAccountSummary",
  "displayName": "Display Name value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "userPrincipalName": "User Principal Name value",
  "osVersion": "Os Version value",
  "successfulUpdateCount": 5,
  "failedUpdateCount": 1,
  "totalUpdateCount": 0,
  "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
}
```

### <a name="response"></a><span data-ttu-id="376f1-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="376f1-171">Response</span></span>
<span data-ttu-id="376f1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="376f1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 502

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateAccountSummary",
  "id": "64687d05-7d05-6468-057d-6864057d6864",
  "displayName": "Display Name value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "userPrincipalName": "User Principal Name value",
  "osVersion": "Os Version value",
  "successfulUpdateCount": 5,
  "failedUpdateCount": 1,
  "totalUpdateCount": 0,
  "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
}
```




