---
title: Criar defaultDeviceCompliancePolicy
description: Criar um novo objeto defaultDeviceCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8b83c040093593565d7f4d2e2b7e7cd575a48951
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37534215"
---
# <a name="create-defaultdevicecompliancepolicy"></a><span data-ttu-id="26d03-103">Criar defaultDeviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="26d03-103">Create defaultDeviceCompliancePolicy</span></span>

> <span data-ttu-id="26d03-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="26d03-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26d03-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="26d03-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26d03-106">Criar um novo objeto [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="26d03-106">Create a new [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26d03-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="26d03-107">Prerequisites</span></span>
<span data-ttu-id="26d03-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26d03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26d03-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26d03-110">Permission type</span></span>|<span data-ttu-id="26d03-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="26d03-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26d03-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26d03-112">Delegated (work or school account)</span></span>|<span data-ttu-id="26d03-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26d03-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="26d03-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26d03-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26d03-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26d03-115">Not supported.</span></span>|
|<span data-ttu-id="26d03-116">Application</span><span class="sxs-lookup"><span data-stu-id="26d03-116">Application</span></span>|<span data-ttu-id="26d03-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26d03-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="26d03-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26d03-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="26d03-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26d03-119">Request headers</span></span>
|<span data-ttu-id="26d03-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="26d03-120">Header</span></span>|<span data-ttu-id="26d03-121">Valor</span><span class="sxs-lookup"><span data-stu-id="26d03-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26d03-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="26d03-122">Authorization</span></span>|<span data-ttu-id="26d03-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26d03-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26d03-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="26d03-124">Accept</span></span>|<span data-ttu-id="26d03-125">application/json</span><span class="sxs-lookup"><span data-stu-id="26d03-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26d03-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26d03-126">Request body</span></span>
<span data-ttu-id="26d03-127">No corpo da solicitação, forneça uma representação JSON do objeto defaultDeviceCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="26d03-127">In the request body, supply a JSON representation for the defaultDeviceCompliancePolicy object.</span></span>

<span data-ttu-id="26d03-128">A tabela a seguir mostra as propriedades que são necessárias ao criar defaultDeviceCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="26d03-128">The following table shows the properties that are required when you create the defaultDeviceCompliancePolicy.</span></span>

|<span data-ttu-id="26d03-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26d03-129">Property</span></span>|<span data-ttu-id="26d03-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="26d03-130">Type</span></span>|<span data-ttu-id="26d03-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="26d03-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26d03-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="26d03-132">roleScopeTagIds</span></span>|<span data-ttu-id="26d03-133">String collection</span><span class="sxs-lookup"><span data-stu-id="26d03-133">String collection</span></span>|<span data-ttu-id="26d03-134">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="26d03-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="26d03-135">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="26d03-135">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="26d03-136">id</span><span class="sxs-lookup"><span data-stu-id="26d03-136">id</span></span>|<span data-ttu-id="26d03-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26d03-137">String</span></span>|<span data-ttu-id="26d03-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="26d03-138">Key of the entity.</span></span> <span data-ttu-id="26d03-139">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="26d03-139">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="26d03-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="26d03-140">createdDateTime</span></span>|<span data-ttu-id="26d03-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26d03-141">DateTimeOffset</span></span>|<span data-ttu-id="26d03-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="26d03-142">DateTime the object was created.</span></span> <span data-ttu-id="26d03-143">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="26d03-143">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="26d03-144">description</span><span class="sxs-lookup"><span data-stu-id="26d03-144">description</span></span>|<span data-ttu-id="26d03-145">String</span><span class="sxs-lookup"><span data-stu-id="26d03-145">String</span></span>|<span data-ttu-id="26d03-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="26d03-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="26d03-147">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="26d03-147">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="26d03-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="26d03-148">lastModifiedDateTime</span></span>|<span data-ttu-id="26d03-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26d03-149">DateTimeOffset</span></span>|<span data-ttu-id="26d03-150">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="26d03-150">DateTime the object was last modified.</span></span> <span data-ttu-id="26d03-151">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="26d03-151">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="26d03-152">displayName</span><span class="sxs-lookup"><span data-stu-id="26d03-152">displayName</span></span>|<span data-ttu-id="26d03-153">String</span><span class="sxs-lookup"><span data-stu-id="26d03-153">String</span></span>|<span data-ttu-id="26d03-154">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="26d03-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="26d03-155">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="26d03-155">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="26d03-156">version</span><span class="sxs-lookup"><span data-stu-id="26d03-156">version</span></span>|<span data-ttu-id="26d03-157">Int32</span><span class="sxs-lookup"><span data-stu-id="26d03-157">Int32</span></span>|<span data-ttu-id="26d03-158">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="26d03-158">Version of the device configuration.</span></span> <span data-ttu-id="26d03-159">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="26d03-159">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="26d03-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="26d03-160">Response</span></span>
<span data-ttu-id="26d03-161">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26d03-161">If successful, this method returns a `201 Created` response code and a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26d03-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26d03-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="26d03-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26d03-163">Request</span></span>
<span data-ttu-id="26d03-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26d03-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 229

{
  "@odata.type": "#microsoft.graph.defaultDeviceCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="26d03-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="26d03-165">Response</span></span>
<span data-ttu-id="26d03-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="26d03-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 401

{
  "@odata.type": "#microsoft.graph.defaultDeviceCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "a285f027-f027-a285-27f0-85a227f085a2",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```






