---
title: Criar networkIPv4ConfigurationManagementCondition
description: Criar um novo objeto networkIPv4ConfigurationManagementCondition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9888bf2bf153413349b03978c0eb9ac0b21457fb
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37179926"
---
# <a name="create-networkipv4configurationmanagementcondition"></a><span data-ttu-id="eda31-103">Criar networkIPv4ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="eda31-103">Create networkIPv4ConfigurationManagementCondition</span></span>

> <span data-ttu-id="eda31-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eda31-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eda31-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eda31-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eda31-106">Criar um novo objeto [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="eda31-106">Create a new [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eda31-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eda31-107">Prerequisites</span></span>
<span data-ttu-id="eda31-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eda31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eda31-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eda31-110">Permission type</span></span>|<span data-ttu-id="eda31-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eda31-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eda31-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eda31-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eda31-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eda31-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eda31-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eda31-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eda31-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eda31-115">Not supported.</span></span>|
|<span data-ttu-id="eda31-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eda31-116">Application</span></span>|<span data-ttu-id="eda31-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eda31-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eda31-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eda31-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="eda31-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eda31-119">Request headers</span></span>
|<span data-ttu-id="eda31-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eda31-120">Header</span></span>|<span data-ttu-id="eda31-121">Valor</span><span class="sxs-lookup"><span data-stu-id="eda31-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eda31-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eda31-122">Authorization</span></span>|<span data-ttu-id="eda31-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eda31-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eda31-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eda31-124">Accept</span></span>|<span data-ttu-id="eda31-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eda31-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eda31-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eda31-126">Request body</span></span>
<span data-ttu-id="eda31-127">No corpo da solicitação, forneça uma representação JSON do objeto networkIPv4ConfigurationManagementCondition.</span><span class="sxs-lookup"><span data-stu-id="eda31-127">In the request body, supply a JSON representation for the networkIPv4ConfigurationManagementCondition object.</span></span>

<span data-ttu-id="eda31-128">A tabela a seguir mostra as propriedades que são necessárias ao criar networkIPv4ConfigurationManagementCondition.</span><span class="sxs-lookup"><span data-stu-id="eda31-128">The following table shows the properties that are required when you create the networkIPv4ConfigurationManagementCondition.</span></span>

|<span data-ttu-id="eda31-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eda31-129">Property</span></span>|<span data-ttu-id="eda31-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="eda31-130">Type</span></span>|<span data-ttu-id="eda31-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="eda31-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eda31-132">id</span><span class="sxs-lookup"><span data-stu-id="eda31-132">id</span></span>|<span data-ttu-id="eda31-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eda31-133">String</span></span>|<span data-ttu-id="eda31-134">Identificador exclusivo da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="eda31-134">Unique identifier for the management condition.</span></span> <span data-ttu-id="eda31-135">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="eda31-135">System generated value assigned when created.</span></span> <span data-ttu-id="eda31-136">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="eda31-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="eda31-137">uniqueName</span><span class="sxs-lookup"><span data-stu-id="eda31-137">uniqueName</span></span>|<span data-ttu-id="eda31-138">String</span><span class="sxs-lookup"><span data-stu-id="eda31-138">String</span></span>|<span data-ttu-id="eda31-139">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="eda31-139">Unique name for the management condition.</span></span> <span data-ttu-id="eda31-140">Usado em expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="eda31-140">Used in management condition expressions.</span></span> <span data-ttu-id="eda31-141">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="eda31-141">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="eda31-142">displayName</span><span class="sxs-lookup"><span data-stu-id="eda31-142">displayName</span></span>|<span data-ttu-id="eda31-143">String</span><span class="sxs-lookup"><span data-stu-id="eda31-143">String</span></span>|<span data-ttu-id="eda31-144">O nome do administrador definido da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="eda31-144">The admin defined name of the management condition.</span></span> <span data-ttu-id="eda31-145">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="eda31-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="eda31-146">descrição</span><span class="sxs-lookup"><span data-stu-id="eda31-146">description</span></span>|<span data-ttu-id="eda31-147">String</span><span class="sxs-lookup"><span data-stu-id="eda31-147">String</span></span>|<span data-ttu-id="eda31-148">A descrição definida pelo administrador da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="eda31-148">The admin defined description of the management condition.</span></span> <span data-ttu-id="eda31-149">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="eda31-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="eda31-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eda31-150">createdDateTime</span></span>|<span data-ttu-id="eda31-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eda31-151">DateTimeOffset</span></span>|<span data-ttu-id="eda31-152">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="eda31-152">The time the management condition was created.</span></span> <span data-ttu-id="eda31-153">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="eda31-153">Generated service side.</span></span> <span data-ttu-id="eda31-154">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="eda31-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="eda31-155">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eda31-155">modifiedDateTime</span></span>|<span data-ttu-id="eda31-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eda31-156">DateTimeOffset</span></span>|<span data-ttu-id="eda31-157">A hora em que a condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="eda31-157">The time the management condition was last modified.</span></span> <span data-ttu-id="eda31-158">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="eda31-158">Updated service side.</span></span> <span data-ttu-id="eda31-159">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="eda31-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="eda31-160">eTag</span><span class="sxs-lookup"><span data-stu-id="eda31-160">eTag</span></span>|<span data-ttu-id="eda31-161">String</span><span class="sxs-lookup"><span data-stu-id="eda31-161">String</span></span>|<span data-ttu-id="eda31-162">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="eda31-162">ETag of the management condition.</span></span> <span data-ttu-id="eda31-163">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="eda31-163">Updated service side.</span></span> <span data-ttu-id="eda31-164">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="eda31-164">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="eda31-165">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="eda31-165">applicablePlatforms</span></span>|<span data-ttu-id="eda31-166">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="eda31-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="eda31-167">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="eda31-167">The applicable platforms for this management condition.</span></span> <span data-ttu-id="eda31-168">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="eda31-168">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="eda31-169">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="eda31-169">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="eda31-170">ipV4Prefix</span><span class="sxs-lookup"><span data-stu-id="eda31-170">ipV4Prefix</span></span>|<span data-ttu-id="eda31-171">String</span><span class="sxs-lookup"><span data-stu-id="eda31-171">String</span></span>|<span data-ttu-id="eda31-172">A sub-rede IPv4 à qual está conectada.</span><span class="sxs-lookup"><span data-stu-id="eda31-172">The IPv4 subnet to be connected to.</span></span> <span data-ttu-id="eda31-173">por exemplo, 10.0.0.0/8</span><span class="sxs-lookup"><span data-stu-id="eda31-173">e.g. 10.0.0.0/8</span></span>|
|<span data-ttu-id="eda31-174">ipV4Gateway</span><span class="sxs-lookup"><span data-stu-id="eda31-174">ipV4Gateway</span></span>|<span data-ttu-id="eda31-175">String</span><span class="sxs-lookup"><span data-stu-id="eda31-175">String</span></span>|<span data-ttu-id="eda31-176">O endereço do gateway IPv4.</span><span class="sxs-lookup"><span data-stu-id="eda31-176">The IPv4 gateway address.</span></span> <span data-ttu-id="eda31-177">por exemplo, 10.0.0.0</span><span class="sxs-lookup"><span data-stu-id="eda31-177">e.g. 10.0.0.0</span></span>|
|<span data-ttu-id="eda31-178">ipV4DHCPServer</span><span class="sxs-lookup"><span data-stu-id="eda31-178">ipV4DHCPServer</span></span>|<span data-ttu-id="eda31-179">String</span><span class="sxs-lookup"><span data-stu-id="eda31-179">String</span></span>|<span data-ttu-id="eda31-180">O endereço IPv4 do servidor DHCP para o adaptador.</span><span class="sxs-lookup"><span data-stu-id="eda31-180">The IPv4 address of the DHCP server for the adapter.</span></span>|
|<span data-ttu-id="eda31-181">ipV4DNSServerList</span><span class="sxs-lookup"><span data-stu-id="eda31-181">ipV4DNSServerList</span></span>|<span data-ttu-id="eda31-182">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="eda31-182">String collection</span></span>|<span data-ttu-id="eda31-183">Os servidores DNS IPv4 configurados para o adaptador.</span><span class="sxs-lookup"><span data-stu-id="eda31-183">The IPv4 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="eda31-184">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="eda31-184">dnsSuffixList</span></span>|<span data-ttu-id="eda31-185">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="eda31-185">String collection</span></span>|<span data-ttu-id="eda31-186">Sufixos DNS válidos para a rede atual.</span><span class="sxs-lookup"><span data-stu-id="eda31-186">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="eda31-187">por exemplo, seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="eda31-187">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="eda31-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="eda31-188">Response</span></span>
<span data-ttu-id="eda31-189">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eda31-189">If successful, this method returns a `201 Created` response code and a [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eda31-190">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eda31-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="eda31-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eda31-191">Request</span></span>
<span data-ttu-id="eda31-192">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eda31-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditions
Content-type: application/json
Content-length: 529

{
  "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV4Prefix": "Ip V4Prefix value",
  "ipV4Gateway": "Ip V4Gateway value",
  "ipV4DHCPServer": "Ip V4DHCPServer value",
  "ipV4DNSServerList": [
    "Ip V4DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="eda31-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="eda31-193">Response</span></span>
<span data-ttu-id="eda31-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eda31-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 697

{
  "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
  "id": "5e4a8284-8284-5e4a-8482-4a5e84824a5e",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV4Prefix": "Ip V4Prefix value",
  "ipV4Gateway": "Ip V4Gateway value",
  "ipV4DHCPServer": "Ip V4DHCPServer value",
  "ipV4DNSServerList": [
    "Ip V4DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```




