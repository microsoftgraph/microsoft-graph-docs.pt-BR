---
title: Atualizar networkIPv6ConfigurationManagementCondition
description: Atualiza as propriedades de um objeto networkIPv6ConfigurationManagementCondition.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ce9b0a3735776995cb24be9a374d81ef44ed06d5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43384210"
---
# <a name="update-networkipv6configurationmanagementcondition"></a><span data-ttu-id="06ca1-103">Atualizar networkIPv6ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="06ca1-103">Update networkIPv6ConfigurationManagementCondition</span></span>

<span data-ttu-id="06ca1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06ca1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06ca1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="06ca1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06ca1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="06ca1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06ca1-107">Atualiza as propriedades de um objeto [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="06ca1-107">Update the properties of a [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06ca1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="06ca1-108">Prerequisites</span></span>
<span data-ttu-id="06ca1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06ca1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06ca1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06ca1-111">Permission type</span></span>|<span data-ttu-id="06ca1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="06ca1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06ca1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06ca1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="06ca1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06ca1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="06ca1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06ca1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06ca1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06ca1-116">Not supported.</span></span>|
|<span data-ttu-id="06ca1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06ca1-117">Application</span></span>|<span data-ttu-id="06ca1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06ca1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="06ca1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06ca1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="06ca1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06ca1-120">Request headers</span></span>
|<span data-ttu-id="06ca1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="06ca1-121">Header</span></span>|<span data-ttu-id="06ca1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="06ca1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06ca1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="06ca1-123">Authorization</span></span>|<span data-ttu-id="06ca1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06ca1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06ca1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="06ca1-125">Accept</span></span>|<span data-ttu-id="06ca1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="06ca1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06ca1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06ca1-127">Request body</span></span>
<span data-ttu-id="06ca1-128">No corpo da solicitação, forneça uma representação JSON do objeto [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="06ca1-128">In the request body, supply a JSON representation for the [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>

<span data-ttu-id="06ca1-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="06ca1-129">The following table shows the properties that are required when you create the [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md).</span></span>

|<span data-ttu-id="06ca1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06ca1-130">Property</span></span>|<span data-ttu-id="06ca1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="06ca1-131">Type</span></span>|<span data-ttu-id="06ca1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="06ca1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06ca1-133">id</span><span class="sxs-lookup"><span data-stu-id="06ca1-133">id</span></span>|<span data-ttu-id="06ca1-134">String</span><span class="sxs-lookup"><span data-stu-id="06ca1-134">String</span></span>|<span data-ttu-id="06ca1-135">Identificador exclusivo da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="06ca1-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="06ca1-136">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="06ca1-136">System generated value assigned when created.</span></span> <span data-ttu-id="06ca1-137">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="06ca1-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="06ca1-138">uniqueName</span><span class="sxs-lookup"><span data-stu-id="06ca1-138">uniqueName</span></span>|<span data-ttu-id="06ca1-139">String</span><span class="sxs-lookup"><span data-stu-id="06ca1-139">String</span></span>|<span data-ttu-id="06ca1-140">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="06ca1-140">Unique name for the management condition.</span></span> <span data-ttu-id="06ca1-141">Usado em expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="06ca1-141">Used in management condition expressions.</span></span> <span data-ttu-id="06ca1-142">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="06ca1-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="06ca1-143">displayName</span><span class="sxs-lookup"><span data-stu-id="06ca1-143">displayName</span></span>|<span data-ttu-id="06ca1-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06ca1-144">String</span></span>|<span data-ttu-id="06ca1-145">O nome do administrador definido da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="06ca1-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="06ca1-146">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="06ca1-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="06ca1-147">description</span><span class="sxs-lookup"><span data-stu-id="06ca1-147">description</span></span>|<span data-ttu-id="06ca1-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06ca1-148">String</span></span>|<span data-ttu-id="06ca1-149">A descrição definida pelo administrador da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="06ca1-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="06ca1-150">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="06ca1-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="06ca1-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06ca1-151">createdDateTime</span></span>|<span data-ttu-id="06ca1-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06ca1-152">DateTimeOffset</span></span>|<span data-ttu-id="06ca1-153">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="06ca1-153">The time the management condition was created.</span></span> <span data-ttu-id="06ca1-154">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="06ca1-154">Generated service side.</span></span> <span data-ttu-id="06ca1-155">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="06ca1-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="06ca1-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06ca1-156">modifiedDateTime</span></span>|<span data-ttu-id="06ca1-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06ca1-157">DateTimeOffset</span></span>|<span data-ttu-id="06ca1-158">A hora em que a condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="06ca1-158">The time the management condition was last modified.</span></span> <span data-ttu-id="06ca1-159">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="06ca1-159">Updated service side.</span></span> <span data-ttu-id="06ca1-160">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="06ca1-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="06ca1-161">eTag</span><span class="sxs-lookup"><span data-stu-id="06ca1-161">eTag</span></span>|<span data-ttu-id="06ca1-162">String</span><span class="sxs-lookup"><span data-stu-id="06ca1-162">String</span></span>|<span data-ttu-id="06ca1-163">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="06ca1-163">ETag of the management condition.</span></span> <span data-ttu-id="06ca1-164">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="06ca1-164">Updated service side.</span></span> <span data-ttu-id="06ca1-165">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="06ca1-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="06ca1-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="06ca1-166">applicablePlatforms</span></span>|<span data-ttu-id="06ca1-167">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="06ca1-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="06ca1-168">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="06ca1-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="06ca1-169">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="06ca1-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="06ca1-170">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="06ca1-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="06ca1-171">ipV6Prefix</span><span class="sxs-lookup"><span data-stu-id="06ca1-171">ipV6Prefix</span></span>|<span data-ttu-id="06ca1-172">String</span><span class="sxs-lookup"><span data-stu-id="06ca1-172">String</span></span>|<span data-ttu-id="06ca1-173">A sub-rede IPv6 a ser conectada.</span><span class="sxs-lookup"><span data-stu-id="06ca1-173">The IPv6 subnet to be connected to.</span></span> <span data-ttu-id="06ca1-174">por exemplo, 2001: DB8::/32</span><span class="sxs-lookup"><span data-stu-id="06ca1-174">e.g. 2001:db8::/32</span></span>|
|<span data-ttu-id="06ca1-175">ipV6Gateway</span><span class="sxs-lookup"><span data-stu-id="06ca1-175">ipV6Gateway</span></span>|<span data-ttu-id="06ca1-176">String</span><span class="sxs-lookup"><span data-stu-id="06ca1-176">String</span></span>|<span data-ttu-id="06ca1-177">O endereço do gateway IPv6 para.</span><span class="sxs-lookup"><span data-stu-id="06ca1-177">The IPv6 gateway address to.</span></span> <span data-ttu-id="06ca1-178">por exemplo, 2001: DB8:: 1</span><span class="sxs-lookup"><span data-stu-id="06ca1-178">e.g 2001:db8::1</span></span>|
|<span data-ttu-id="06ca1-179">ipV6DNSServerList</span><span class="sxs-lookup"><span data-stu-id="06ca1-179">ipV6DNSServerList</span></span>|<span data-ttu-id="06ca1-180">Coleção String</span><span class="sxs-lookup"><span data-stu-id="06ca1-180">String collection</span></span>|<span data-ttu-id="06ca1-181">Servidores DNS IPv6 configurados para o adaptador.</span><span class="sxs-lookup"><span data-stu-id="06ca1-181">An IPv6 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="06ca1-182">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="06ca1-182">dnsSuffixList</span></span>|<span data-ttu-id="06ca1-183">Coleção String</span><span class="sxs-lookup"><span data-stu-id="06ca1-183">String collection</span></span>|<span data-ttu-id="06ca1-184">Sufixos DNS válidos para a rede atual.</span><span class="sxs-lookup"><span data-stu-id="06ca1-184">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="06ca1-185">por exemplo, seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="06ca1-185">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="06ca1-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="06ca1-186">Response</span></span>
<span data-ttu-id="06ca1-187">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06ca1-187">If successful, this method returns a `200 OK` response code and an updated [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06ca1-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06ca1-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="06ca1-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06ca1-189">Request</span></span>
<span data-ttu-id="06ca1-190">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06ca1-190">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
Content-type: application/json
Content-length: 483

{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV6Prefix": "Ip V6Prefix value",
  "ipV6Gateway": "Ip V6Gateway value",
  "ipV6DNSServerList": [
    "Ip V6DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="06ca1-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="06ca1-191">Response</span></span>
<span data-ttu-id="06ca1-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06ca1-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 651

{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
  "id": "25811206-1206-2581-0612-812506128125",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV6Prefix": "Ip V6Prefix value",
  "ipV6Gateway": "Ip V6Gateway value",
  "ipV6DNSServerList": [
    "Ip V6DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```



