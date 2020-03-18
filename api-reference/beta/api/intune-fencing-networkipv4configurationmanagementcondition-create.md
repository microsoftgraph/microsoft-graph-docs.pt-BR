---
title: Criar networkIPv4ConfigurationManagementCondition
description: Criar um novo objeto networkIPv4ConfigurationManagementCondition.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 999f23f4a2e1164a3861d344cad8b5d334842388
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804720"
---
# <a name="create-networkipv4configurationmanagementcondition"></a><span data-ttu-id="4c259-103">Criar networkIPv4ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="4c259-103">Create networkIPv4ConfigurationManagementCondition</span></span>

> <span data-ttu-id="4c259-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4c259-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c259-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4c259-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c259-106">Criar um novo objeto [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="4c259-106">Create a new [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c259-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4c259-107">Prerequisites</span></span>
<span data-ttu-id="4c259-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c259-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c259-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c259-110">Permission type</span></span>|<span data-ttu-id="4c259-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4c259-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c259-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c259-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4c259-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c259-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4c259-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c259-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c259-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c259-115">Not supported.</span></span>|
|<span data-ttu-id="4c259-116">Application</span><span class="sxs-lookup"><span data-stu-id="4c259-116">Application</span></span>|<span data-ttu-id="4c259-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c259-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c259-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c259-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="4c259-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c259-119">Request headers</span></span>
|<span data-ttu-id="4c259-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4c259-120">Header</span></span>|<span data-ttu-id="4c259-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4c259-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c259-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c259-122">Authorization</span></span>|<span data-ttu-id="4c259-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c259-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c259-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4c259-124">Accept</span></span>|<span data-ttu-id="4c259-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4c259-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c259-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c259-126">Request body</span></span>
<span data-ttu-id="4c259-127">No corpo da solicitação, forneça uma representação JSON do objeto networkIPv4ConfigurationManagementCondition.</span><span class="sxs-lookup"><span data-stu-id="4c259-127">In the request body, supply a JSON representation for the networkIPv4ConfigurationManagementCondition object.</span></span>

<span data-ttu-id="4c259-128">A tabela a seguir mostra as propriedades que são necessárias ao criar networkIPv4ConfigurationManagementCondition.</span><span class="sxs-lookup"><span data-stu-id="4c259-128">The following table shows the properties that are required when you create the networkIPv4ConfigurationManagementCondition.</span></span>

|<span data-ttu-id="4c259-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4c259-129">Property</span></span>|<span data-ttu-id="4c259-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c259-130">Type</span></span>|<span data-ttu-id="4c259-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c259-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c259-132">id</span><span class="sxs-lookup"><span data-stu-id="4c259-132">id</span></span>|<span data-ttu-id="4c259-133">String</span><span class="sxs-lookup"><span data-stu-id="4c259-133">String</span></span>|<span data-ttu-id="4c259-134">Identificador exclusivo da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="4c259-134">Unique identifier for the management condition.</span></span> <span data-ttu-id="4c259-135">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="4c259-135">System generated value assigned when created.</span></span> <span data-ttu-id="4c259-136">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="4c259-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="4c259-137">uniqueName</span><span class="sxs-lookup"><span data-stu-id="4c259-137">uniqueName</span></span>|<span data-ttu-id="4c259-138">String</span><span class="sxs-lookup"><span data-stu-id="4c259-138">String</span></span>|<span data-ttu-id="4c259-139">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="4c259-139">Unique name for the management condition.</span></span> <span data-ttu-id="4c259-140">Usado em expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="4c259-140">Used in management condition expressions.</span></span> <span data-ttu-id="4c259-141">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="4c259-141">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="4c259-142">displayName</span><span class="sxs-lookup"><span data-stu-id="4c259-142">displayName</span></span>|<span data-ttu-id="4c259-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c259-143">String</span></span>|<span data-ttu-id="4c259-144">O nome do administrador definido da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="4c259-144">The admin defined name of the management condition.</span></span> <span data-ttu-id="4c259-145">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="4c259-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="4c259-146">description</span><span class="sxs-lookup"><span data-stu-id="4c259-146">description</span></span>|<span data-ttu-id="4c259-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c259-147">String</span></span>|<span data-ttu-id="4c259-148">A descrição definida pelo administrador da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="4c259-148">The admin defined description of the management condition.</span></span> <span data-ttu-id="4c259-149">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="4c259-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="4c259-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4c259-150">createdDateTime</span></span>|<span data-ttu-id="4c259-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c259-151">DateTimeOffset</span></span>|<span data-ttu-id="4c259-152">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="4c259-152">The time the management condition was created.</span></span> <span data-ttu-id="4c259-153">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="4c259-153">Generated service side.</span></span> <span data-ttu-id="4c259-154">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="4c259-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="4c259-155">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4c259-155">modifiedDateTime</span></span>|<span data-ttu-id="4c259-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c259-156">DateTimeOffset</span></span>|<span data-ttu-id="4c259-157">A hora em que a condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="4c259-157">The time the management condition was last modified.</span></span> <span data-ttu-id="4c259-158">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="4c259-158">Updated service side.</span></span> <span data-ttu-id="4c259-159">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="4c259-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="4c259-160">eTag</span><span class="sxs-lookup"><span data-stu-id="4c259-160">eTag</span></span>|<span data-ttu-id="4c259-161">String</span><span class="sxs-lookup"><span data-stu-id="4c259-161">String</span></span>|<span data-ttu-id="4c259-162">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="4c259-162">ETag of the management condition.</span></span> <span data-ttu-id="4c259-163">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="4c259-163">Updated service side.</span></span> <span data-ttu-id="4c259-164">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="4c259-164">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="4c259-165">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="4c259-165">applicablePlatforms</span></span>|<span data-ttu-id="4c259-166">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="4c259-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="4c259-167">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="4c259-167">The applicable platforms for this management condition.</span></span> <span data-ttu-id="4c259-168">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="4c259-168">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="4c259-169">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="4c259-169">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="4c259-170">ipV4Prefix</span><span class="sxs-lookup"><span data-stu-id="4c259-170">ipV4Prefix</span></span>|<span data-ttu-id="4c259-171">String</span><span class="sxs-lookup"><span data-stu-id="4c259-171">String</span></span>|<span data-ttu-id="4c259-172">A sub-rede IPv4 à qual está conectada.</span><span class="sxs-lookup"><span data-stu-id="4c259-172">The IPv4 subnet to be connected to.</span></span> <span data-ttu-id="4c259-173">por exemplo, 10.0.0.0/8</span><span class="sxs-lookup"><span data-stu-id="4c259-173">e.g. 10.0.0.0/8</span></span>|
|<span data-ttu-id="4c259-174">ipV4Gateway</span><span class="sxs-lookup"><span data-stu-id="4c259-174">ipV4Gateway</span></span>|<span data-ttu-id="4c259-175">String</span><span class="sxs-lookup"><span data-stu-id="4c259-175">String</span></span>|<span data-ttu-id="4c259-176">O endereço do gateway IPv4.</span><span class="sxs-lookup"><span data-stu-id="4c259-176">The IPv4 gateway address.</span></span> <span data-ttu-id="4c259-177">por exemplo, 10.0.0.0</span><span class="sxs-lookup"><span data-stu-id="4c259-177">e.g. 10.0.0.0</span></span>|
|<span data-ttu-id="4c259-178">ipV4DHCPServer</span><span class="sxs-lookup"><span data-stu-id="4c259-178">ipV4DHCPServer</span></span>|<span data-ttu-id="4c259-179">String</span><span class="sxs-lookup"><span data-stu-id="4c259-179">String</span></span>|<span data-ttu-id="4c259-180">O endereço IPv4 do servidor DHCP para o adaptador.</span><span class="sxs-lookup"><span data-stu-id="4c259-180">The IPv4 address of the DHCP server for the adapter.</span></span>|
|<span data-ttu-id="4c259-181">ipV4DNSServerList</span><span class="sxs-lookup"><span data-stu-id="4c259-181">ipV4DNSServerList</span></span>|<span data-ttu-id="4c259-182">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c259-182">String collection</span></span>|<span data-ttu-id="4c259-183">Os servidores DNS IPv4 configurados para o adaptador.</span><span class="sxs-lookup"><span data-stu-id="4c259-183">The IPv4 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="4c259-184">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="4c259-184">dnsSuffixList</span></span>|<span data-ttu-id="4c259-185">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c259-185">String collection</span></span>|<span data-ttu-id="4c259-186">Sufixos DNS válidos para a rede atual.</span><span class="sxs-lookup"><span data-stu-id="4c259-186">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="4c259-187">por exemplo, seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="4c259-187">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="4c259-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c259-188">Response</span></span>
<span data-ttu-id="4c259-189">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c259-189">If successful, this method returns a `201 Created` response code and a [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c259-190">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c259-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c259-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c259-191">Request</span></span>
<span data-ttu-id="4c259-192">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c259-192">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4c259-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c259-193">Response</span></span>
<span data-ttu-id="4c259-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4c259-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




