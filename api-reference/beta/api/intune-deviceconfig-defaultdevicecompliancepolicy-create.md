---
title: Criar defaultDeviceCompliancePolicy
description: Criar um novo objeto defaultDeviceCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 183893bb3d07833964cd3f310a6c9051ff95c05a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33928033"
---
# <a name="create-defaultdevicecompliancepolicy"></a><span data-ttu-id="493fc-103">Criar defaultDeviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="493fc-103">Create defaultDeviceCompliancePolicy</span></span>

> <span data-ttu-id="493fc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="493fc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="493fc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="493fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="493fc-106">Criar um novo objeto [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="493fc-106">Create a new [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="493fc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="493fc-107">Prerequisites</span></span>
<span data-ttu-id="493fc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="493fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="493fc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="493fc-110">Permission type</span></span>|<span data-ttu-id="493fc-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="493fc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="493fc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="493fc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="493fc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="493fc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="493fc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="493fc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="493fc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="493fc-115">Not supported.</span></span>|
|<span data-ttu-id="493fc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="493fc-116">Application</span></span>|<span data-ttu-id="493fc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="493fc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="493fc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="493fc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="493fc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="493fc-119">Request headers</span></span>
|<span data-ttu-id="493fc-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="493fc-120">Header</span></span>|<span data-ttu-id="493fc-121">Valor</span><span class="sxs-lookup"><span data-stu-id="493fc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="493fc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="493fc-122">Authorization</span></span>|<span data-ttu-id="493fc-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="493fc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="493fc-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="493fc-124">Accept</span></span>|<span data-ttu-id="493fc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="493fc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="493fc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="493fc-126">Request body</span></span>
<span data-ttu-id="493fc-127">No corpo da solicitação, forneça uma representação JSON do objeto defaultDeviceCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="493fc-127">In the request body, supply a JSON representation for the defaultDeviceCompliancePolicy object.</span></span>

<span data-ttu-id="493fc-128">A tabela a seguir mostra as propriedades que são necessárias ao criar defaultDeviceCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="493fc-128">The following table shows the properties that are required when you create the defaultDeviceCompliancePolicy.</span></span>

|<span data-ttu-id="493fc-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="493fc-129">Property</span></span>|<span data-ttu-id="493fc-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="493fc-130">Type</span></span>|<span data-ttu-id="493fc-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="493fc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="493fc-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="493fc-132">roleScopeTagIds</span></span>|<span data-ttu-id="493fc-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="493fc-133">String collection</span></span>|<span data-ttu-id="493fc-134">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="493fc-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="493fc-135">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="493fc-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="493fc-136">id</span><span class="sxs-lookup"><span data-stu-id="493fc-136">id</span></span>|<span data-ttu-id="493fc-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="493fc-137">String</span></span>|<span data-ttu-id="493fc-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="493fc-138">Key of the entity.</span></span> <span data-ttu-id="493fc-139">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="493fc-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="493fc-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="493fc-140">createdDateTime</span></span>|<span data-ttu-id="493fc-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="493fc-141">DateTimeOffset</span></span>|<span data-ttu-id="493fc-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="493fc-142">DateTime the object was created.</span></span> <span data-ttu-id="493fc-143">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="493fc-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="493fc-144">description</span><span class="sxs-lookup"><span data-stu-id="493fc-144">description</span></span>|<span data-ttu-id="493fc-145">String</span><span class="sxs-lookup"><span data-stu-id="493fc-145">String</span></span>|<span data-ttu-id="493fc-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="493fc-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="493fc-147">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="493fc-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="493fc-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="493fc-148">lastModifiedDateTime</span></span>|<span data-ttu-id="493fc-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="493fc-149">DateTimeOffset</span></span>|<span data-ttu-id="493fc-150">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="493fc-150">DateTime the object was last modified.</span></span> <span data-ttu-id="493fc-151">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="493fc-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="493fc-152">displayName</span><span class="sxs-lookup"><span data-stu-id="493fc-152">displayName</span></span>|<span data-ttu-id="493fc-153">String</span><span class="sxs-lookup"><span data-stu-id="493fc-153">String</span></span>|<span data-ttu-id="493fc-154">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="493fc-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="493fc-155">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="493fc-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="493fc-156">version</span><span class="sxs-lookup"><span data-stu-id="493fc-156">version</span></span>|<span data-ttu-id="493fc-157">Int32</span><span class="sxs-lookup"><span data-stu-id="493fc-157">Int32</span></span>|<span data-ttu-id="493fc-158">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="493fc-158">Version of the device configuration.</span></span> <span data-ttu-id="493fc-159">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="493fc-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="493fc-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="493fc-160">Response</span></span>
<span data-ttu-id="493fc-161">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="493fc-161">If successful, this method returns a `201 Created` response code and a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="493fc-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="493fc-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="493fc-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="493fc-163">Request</span></span>
<span data-ttu-id="493fc-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="493fc-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="493fc-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="493fc-165">Response</span></span>
<span data-ttu-id="493fc-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="493fc-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




