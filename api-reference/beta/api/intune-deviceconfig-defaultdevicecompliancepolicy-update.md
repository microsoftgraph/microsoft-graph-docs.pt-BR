---
title: Atualizar defaultDeviceCompliancePolicy
description: Atualiza as propriedades de um objeto defaultDeviceCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 27c3aedeaf17f26a3144c7bf5daff3a826960bb6
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34968676"
---
# <a name="update-defaultdevicecompliancepolicy"></a><span data-ttu-id="6162f-103">Atualizar defaultDeviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="6162f-103">Update defaultDeviceCompliancePolicy</span></span>

> <span data-ttu-id="6162f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6162f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6162f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6162f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6162f-106">Atualiza as propriedades de um objeto [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="6162f-106">Update the properties of a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6162f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6162f-107">Prerequisites</span></span>
<span data-ttu-id="6162f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6162f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6162f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6162f-110">Permission type</span></span>|<span data-ttu-id="6162f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6162f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6162f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6162f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6162f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6162f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6162f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6162f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6162f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6162f-115">Not supported.</span></span>|
|<span data-ttu-id="6162f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6162f-116">Application</span></span>|<span data-ttu-id="6162f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6162f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6162f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6162f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="6162f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6162f-119">Request headers</span></span>
|<span data-ttu-id="6162f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6162f-120">Header</span></span>|<span data-ttu-id="6162f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6162f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6162f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6162f-122">Authorization</span></span>|<span data-ttu-id="6162f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6162f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6162f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6162f-124">Accept</span></span>|<span data-ttu-id="6162f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6162f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6162f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6162f-126">Request body</span></span>
<span data-ttu-id="6162f-127">No corpo da solicitação, forneça uma representação JSON do objeto [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="6162f-127">In the request body, supply a JSON representation for the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

<span data-ttu-id="6162f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6162f-128">The following table shows the properties that are required when you create the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span></span>

|<span data-ttu-id="6162f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6162f-129">Property</span></span>|<span data-ttu-id="6162f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6162f-130">Type</span></span>|<span data-ttu-id="6162f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6162f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6162f-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6162f-132">roleScopeTagIds</span></span>|<span data-ttu-id="6162f-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6162f-133">String collection</span></span>|<span data-ttu-id="6162f-134">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="6162f-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6162f-135">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6162f-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6162f-136">id</span><span class="sxs-lookup"><span data-stu-id="6162f-136">id</span></span>|<span data-ttu-id="6162f-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6162f-137">String</span></span>|<span data-ttu-id="6162f-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6162f-138">Key of the entity.</span></span> <span data-ttu-id="6162f-139">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6162f-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6162f-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6162f-140">createdDateTime</span></span>|<span data-ttu-id="6162f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6162f-141">DateTimeOffset</span></span>|<span data-ttu-id="6162f-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6162f-142">DateTime the object was created.</span></span> <span data-ttu-id="6162f-143">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6162f-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6162f-144">descrição</span><span class="sxs-lookup"><span data-stu-id="6162f-144">description</span></span>|<span data-ttu-id="6162f-145">String</span><span class="sxs-lookup"><span data-stu-id="6162f-145">String</span></span>|<span data-ttu-id="6162f-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6162f-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6162f-147">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6162f-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6162f-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6162f-148">lastModifiedDateTime</span></span>|<span data-ttu-id="6162f-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6162f-149">DateTimeOffset</span></span>|<span data-ttu-id="6162f-150">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6162f-150">DateTime the object was last modified.</span></span> <span data-ttu-id="6162f-151">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6162f-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6162f-152">displayName</span><span class="sxs-lookup"><span data-stu-id="6162f-152">displayName</span></span>|<span data-ttu-id="6162f-153">String</span><span class="sxs-lookup"><span data-stu-id="6162f-153">String</span></span>|<span data-ttu-id="6162f-154">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6162f-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6162f-155">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6162f-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6162f-156">version</span><span class="sxs-lookup"><span data-stu-id="6162f-156">version</span></span>|<span data-ttu-id="6162f-157">Int32</span><span class="sxs-lookup"><span data-stu-id="6162f-157">Int32</span></span>|<span data-ttu-id="6162f-158">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6162f-158">Version of the device configuration.</span></span> <span data-ttu-id="6162f-159">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6162f-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="6162f-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="6162f-160">Response</span></span>
<span data-ttu-id="6162f-161">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6162f-161">If successful, this method returns a `200 OK` response code and an updated [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6162f-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6162f-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="6162f-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6162f-163">Request</span></span>
<span data-ttu-id="6162f-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6162f-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6162f-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="6162f-165">Response</span></span>
<span data-ttu-id="6162f-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6162f-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





