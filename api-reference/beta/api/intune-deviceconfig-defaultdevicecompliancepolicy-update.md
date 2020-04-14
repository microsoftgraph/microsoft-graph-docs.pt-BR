---
title: Atualizar defaultDeviceCompliancePolicy
description: Atualiza as propriedades de um objeto defaultDeviceCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ac0799c8065d2cc8dee12f4fe9bc5cf3a6e4932d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43434286"
---
# <a name="update-defaultdevicecompliancepolicy"></a><span data-ttu-id="8c603-103">Atualizar defaultDeviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="8c603-103">Update defaultDeviceCompliancePolicy</span></span>

<span data-ttu-id="8c603-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c603-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c603-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8c603-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c603-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8c603-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c603-107">Atualiza as propriedades de um objeto [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="8c603-107">Update the properties of a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c603-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8c603-108">Prerequisites</span></span>
<span data-ttu-id="8c603-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c603-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c603-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c603-111">Permission type</span></span>|<span data-ttu-id="8c603-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8c603-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c603-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c603-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8c603-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c603-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8c603-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c603-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c603-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c603-116">Not supported.</span></span>|
|<span data-ttu-id="8c603-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c603-117">Application</span></span>|<span data-ttu-id="8c603-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c603-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c603-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c603-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="8c603-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c603-120">Request headers</span></span>
|<span data-ttu-id="8c603-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8c603-121">Header</span></span>|<span data-ttu-id="8c603-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8c603-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c603-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c603-123">Authorization</span></span>|<span data-ttu-id="8c603-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c603-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c603-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8c603-125">Accept</span></span>|<span data-ttu-id="8c603-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8c603-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c603-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c603-127">Request body</span></span>
<span data-ttu-id="8c603-128">No corpo da solicitação, forneça uma representação JSON do objeto [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="8c603-128">In the request body, supply a JSON representation for the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

<span data-ttu-id="8c603-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8c603-129">The following table shows the properties that are required when you create the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span></span>

|<span data-ttu-id="8c603-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c603-130">Property</span></span>|<span data-ttu-id="8c603-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c603-131">Type</span></span>|<span data-ttu-id="8c603-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c603-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c603-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8c603-133">roleScopeTagIds</span></span>|<span data-ttu-id="8c603-134">Coleção String</span><span class="sxs-lookup"><span data-stu-id="8c603-134">String collection</span></span>|<span data-ttu-id="8c603-135">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="8c603-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8c603-136">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8c603-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8c603-137">id</span><span class="sxs-lookup"><span data-stu-id="8c603-137">id</span></span>|<span data-ttu-id="8c603-138">String</span><span class="sxs-lookup"><span data-stu-id="8c603-138">String</span></span>|<span data-ttu-id="8c603-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8c603-139">Key of the entity.</span></span> <span data-ttu-id="8c603-140">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8c603-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8c603-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8c603-141">createdDateTime</span></span>|<span data-ttu-id="8c603-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c603-142">DateTimeOffset</span></span>|<span data-ttu-id="8c603-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="8c603-143">DateTime the object was created.</span></span> <span data-ttu-id="8c603-144">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8c603-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8c603-145">description</span><span class="sxs-lookup"><span data-stu-id="8c603-145">description</span></span>|<span data-ttu-id="8c603-146">String</span><span class="sxs-lookup"><span data-stu-id="8c603-146">String</span></span>|<span data-ttu-id="8c603-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8c603-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8c603-148">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8c603-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8c603-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8c603-149">lastModifiedDateTime</span></span>|<span data-ttu-id="8c603-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c603-150">DateTimeOffset</span></span>|<span data-ttu-id="8c603-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="8c603-151">DateTime the object was last modified.</span></span> <span data-ttu-id="8c603-152">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8c603-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8c603-153">displayName</span><span class="sxs-lookup"><span data-stu-id="8c603-153">displayName</span></span>|<span data-ttu-id="8c603-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c603-154">String</span></span>|<span data-ttu-id="8c603-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8c603-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8c603-156">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8c603-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8c603-157">version</span><span class="sxs-lookup"><span data-stu-id="8c603-157">version</span></span>|<span data-ttu-id="8c603-158">Int32</span><span class="sxs-lookup"><span data-stu-id="8c603-158">Int32</span></span>|<span data-ttu-id="8c603-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8c603-159">Version of the device configuration.</span></span> <span data-ttu-id="8c603-160">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8c603-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="8c603-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c603-161">Response</span></span>
<span data-ttu-id="8c603-162">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c603-162">If successful, this method returns a `200 OK` response code and an updated [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c603-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c603-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c603-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c603-164">Request</span></span>
<span data-ttu-id="8c603-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c603-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8c603-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c603-166">Response</span></span>
<span data-ttu-id="8c603-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8c603-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



