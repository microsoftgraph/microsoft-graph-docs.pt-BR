---
title: Atualizar defaultDeviceCompliancePolicy
description: Atualiza as propriedades de um objeto defaultDeviceCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fdfb957022d66a4e4e18209d6ba9b8a3c0e776f0
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949802"
---
# <a name="update-defaultdevicecompliancepolicy"></a><span data-ttu-id="7180e-103">Atualizar defaultDeviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="7180e-103">Update defaultDeviceCompliancePolicy</span></span>

> <span data-ttu-id="7180e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7180e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7180e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7180e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7180e-106">Atualiza as propriedades de um objeto [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="7180e-106">Update the properties of a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7180e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7180e-107">Prerequisites</span></span>
<span data-ttu-id="7180e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7180e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7180e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7180e-110">Permission type</span></span>|<span data-ttu-id="7180e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7180e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7180e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7180e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7180e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7180e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7180e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7180e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7180e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7180e-115">Not supported.</span></span>|
|<span data-ttu-id="7180e-116">Application</span><span class="sxs-lookup"><span data-stu-id="7180e-116">Application</span></span>|<span data-ttu-id="7180e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7180e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7180e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7180e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="7180e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7180e-119">Request headers</span></span>
|<span data-ttu-id="7180e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7180e-120">Header</span></span>|<span data-ttu-id="7180e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7180e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7180e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7180e-122">Authorization</span></span>|<span data-ttu-id="7180e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7180e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7180e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7180e-124">Accept</span></span>|<span data-ttu-id="7180e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7180e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7180e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7180e-126">Request body</span></span>
<span data-ttu-id="7180e-127">No corpo da solicitação, forneça uma representação JSON do objeto [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="7180e-127">In the request body, supply a JSON representation for the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

<span data-ttu-id="7180e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7180e-128">The following table shows the properties that are required when you create the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span></span>

|<span data-ttu-id="7180e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7180e-129">Property</span></span>|<span data-ttu-id="7180e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7180e-130">Type</span></span>|<span data-ttu-id="7180e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7180e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7180e-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7180e-132">roleScopeTagIds</span></span>|<span data-ttu-id="7180e-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7180e-133">String collection</span></span>|<span data-ttu-id="7180e-134">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="7180e-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7180e-135">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7180e-135">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7180e-136">id</span><span class="sxs-lookup"><span data-stu-id="7180e-136">id</span></span>|<span data-ttu-id="7180e-137">String</span><span class="sxs-lookup"><span data-stu-id="7180e-137">String</span></span>|<span data-ttu-id="7180e-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7180e-138">Key of the entity.</span></span> <span data-ttu-id="7180e-139">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7180e-139">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7180e-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7180e-140">createdDateTime</span></span>|<span data-ttu-id="7180e-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7180e-141">DateTimeOffset</span></span>|<span data-ttu-id="7180e-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="7180e-142">DateTime the object was created.</span></span> <span data-ttu-id="7180e-143">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7180e-143">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7180e-144">description</span><span class="sxs-lookup"><span data-stu-id="7180e-144">description</span></span>|<span data-ttu-id="7180e-145">String</span><span class="sxs-lookup"><span data-stu-id="7180e-145">String</span></span>|<span data-ttu-id="7180e-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7180e-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7180e-147">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7180e-147">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7180e-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7180e-148">lastModifiedDateTime</span></span>|<span data-ttu-id="7180e-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7180e-149">DateTimeOffset</span></span>|<span data-ttu-id="7180e-150">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="7180e-150">DateTime the object was last modified.</span></span> <span data-ttu-id="7180e-151">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7180e-151">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7180e-152">displayName</span><span class="sxs-lookup"><span data-stu-id="7180e-152">displayName</span></span>|<span data-ttu-id="7180e-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7180e-153">String</span></span>|<span data-ttu-id="7180e-154">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7180e-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7180e-155">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7180e-155">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7180e-156">version</span><span class="sxs-lookup"><span data-stu-id="7180e-156">version</span></span>|<span data-ttu-id="7180e-157">Int32</span><span class="sxs-lookup"><span data-stu-id="7180e-157">Int32</span></span>|<span data-ttu-id="7180e-158">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7180e-158">Version of the device configuration.</span></span> <span data-ttu-id="7180e-159">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7180e-159">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="7180e-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="7180e-160">Response</span></span>
<span data-ttu-id="7180e-161">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7180e-161">If successful, this method returns a `200 OK` response code and an updated [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7180e-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7180e-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="7180e-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7180e-163">Request</span></span>
<span data-ttu-id="7180e-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7180e-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
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

### <a name="response"></a><span data-ttu-id="7180e-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="7180e-165">Response</span></span>
<span data-ttu-id="7180e-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7180e-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





