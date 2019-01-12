---
title: Atualizar networkIPv4ConfigurationManagementCondition
description: Atualize as propriedades de um objeto networkIPv4ConfigurationManagementCondition.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 305e8ff97b54db0888842fdbd60f88ab2ee0677e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953151"
---
# <a name="update-networkipv4configurationmanagementcondition"></a><span data-ttu-id="068e1-103">Atualizar networkIPv4ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="068e1-103">Update networkIPv4ConfigurationManagementCondition</span></span>

> <span data-ttu-id="068e1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="068e1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="068e1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="068e1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="068e1-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="068e1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="068e1-107">Atualize as propriedades de um objeto [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="068e1-107">Update the properties of a [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="068e1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="068e1-108">Prerequisites</span></span>
<span data-ttu-id="068e1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="068e1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="068e1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="068e1-111">Permission type</span></span>|<span data-ttu-id="068e1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="068e1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="068e1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="068e1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="068e1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="068e1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="068e1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="068e1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="068e1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="068e1-116">Not supported.</span></span>|
|<span data-ttu-id="068e1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="068e1-117">Application</span></span>|<span data-ttu-id="068e1-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="068e1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="068e1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="068e1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="068e1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="068e1-120">Request headers</span></span>
|<span data-ttu-id="068e1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="068e1-121">Header</span></span>|<span data-ttu-id="068e1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="068e1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="068e1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="068e1-123">Authorization</span></span>|<span data-ttu-id="068e1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="068e1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="068e1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="068e1-125">Accept</span></span>|<span data-ttu-id="068e1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="068e1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="068e1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="068e1-127">Request body</span></span>
<span data-ttu-id="068e1-128">No corpo da solicitação, fornece uma representação JSON para o objeto [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="068e1-128">In the request body, supply a JSON representation for the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

<span data-ttu-id="068e1-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="068e1-129">The following table shows the properties that are required when you create the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md).</span></span>

|<span data-ttu-id="068e1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="068e1-130">Property</span></span>|<span data-ttu-id="068e1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="068e1-131">Type</span></span>|<span data-ttu-id="068e1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="068e1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="068e1-133">id</span><span class="sxs-lookup"><span data-stu-id="068e1-133">id</span></span>|<span data-ttu-id="068e1-134">String</span><span class="sxs-lookup"><span data-stu-id="068e1-134">String</span></span>|<span data-ttu-id="068e1-135">Identificador exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="068e1-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="068e1-136">Valor atribuído quando criado gerado pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="068e1-136">System generated value assigned when created.</span></span> <span data-ttu-id="068e1-137">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="068e1-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="068e1-138">nome exclusivo</span><span class="sxs-lookup"><span data-stu-id="068e1-138">uniqueName</span></span>|<span data-ttu-id="068e1-139">String</span><span class="sxs-lookup"><span data-stu-id="068e1-139">String</span></span>|<span data-ttu-id="068e1-140">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="068e1-140">Unique name for the management condition.</span></span> <span data-ttu-id="068e1-141">Usadas nas expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="068e1-141">Used in management condition expressions.</span></span> <span data-ttu-id="068e1-142">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="068e1-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="068e1-143">displayName</span><span class="sxs-lookup"><span data-stu-id="068e1-143">displayName</span></span>|<span data-ttu-id="068e1-144">String</span><span class="sxs-lookup"><span data-stu-id="068e1-144">String</span></span>|<span data-ttu-id="068e1-145">O nome definido admin da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="068e1-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="068e1-146">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="068e1-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="068e1-147">description</span><span class="sxs-lookup"><span data-stu-id="068e1-147">description</span></span>|<span data-ttu-id="068e1-148">String</span><span class="sxs-lookup"><span data-stu-id="068e1-148">String</span></span>|<span data-ttu-id="068e1-149">O administrador definidos descrição da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="068e1-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="068e1-150">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="068e1-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="068e1-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="068e1-151">createdDateTime</span></span>|<span data-ttu-id="068e1-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="068e1-152">DateTimeOffset</span></span>|<span data-ttu-id="068e1-153">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="068e1-153">The time the management condition was created.</span></span> <span data-ttu-id="068e1-154">Lado de serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="068e1-154">Generated service side.</span></span> <span data-ttu-id="068e1-155">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="068e1-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="068e1-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="068e1-156">modifiedDateTime</span></span>|<span data-ttu-id="068e1-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="068e1-157">DateTimeOffset</span></span>|<span data-ttu-id="068e1-158">A hora que da última modificação a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="068e1-158">The time the management condition was last modified.</span></span> <span data-ttu-id="068e1-159">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="068e1-159">Updated service side.</span></span> <span data-ttu-id="068e1-160">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="068e1-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="068e1-161">eTag</span><span class="sxs-lookup"><span data-stu-id="068e1-161">eTag</span></span>|<span data-ttu-id="068e1-162">String</span><span class="sxs-lookup"><span data-stu-id="068e1-162">String</span></span>|<span data-ttu-id="068e1-163">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="068e1-163">ETag of the management condition.</span></span> <span data-ttu-id="068e1-164">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="068e1-164">Updated service side.</span></span> <span data-ttu-id="068e1-165">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="068e1-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="068e1-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="068e1-166">applicablePlatforms</span></span>|<span data-ttu-id="068e1-167">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="068e1-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="068e1-168">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="068e1-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="068e1-169">Herdada do [managementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="068e1-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="068e1-170">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="068e1-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="068e1-171">ipV4Prefix</span><span class="sxs-lookup"><span data-stu-id="068e1-171">ipV4Prefix</span></span>|<span data-ttu-id="068e1-172">String</span><span class="sxs-lookup"><span data-stu-id="068e1-172">String</span></span>|<span data-ttu-id="068e1-173">A sub-rede IPv4 seja conectada.</span><span class="sxs-lookup"><span data-stu-id="068e1-173">The IPv4 subnet to be connected to.</span></span> <span data-ttu-id="068e1-174">Por exemplo, 10.0.0.0/8</span><span class="sxs-lookup"><span data-stu-id="068e1-174">e.g. 10.0.0.0/8</span></span>|
|<span data-ttu-id="068e1-175">ipV4Gateway</span><span class="sxs-lookup"><span data-stu-id="068e1-175">ipV4Gateway</span></span>|<span data-ttu-id="068e1-176">String</span><span class="sxs-lookup"><span data-stu-id="068e1-176">String</span></span>|<span data-ttu-id="068e1-177">O endereço de gateway IPv4.</span><span class="sxs-lookup"><span data-stu-id="068e1-177">The IPv4 gateway address.</span></span> <span data-ttu-id="068e1-178">Por exemplo, 10.0.0.0</span><span class="sxs-lookup"><span data-stu-id="068e1-178">e.g. 10.0.0.0</span></span>|
|<span data-ttu-id="068e1-179">ipV4DHCPServer</span><span class="sxs-lookup"><span data-stu-id="068e1-179">ipV4DHCPServer</span></span>|<span data-ttu-id="068e1-180">String</span><span class="sxs-lookup"><span data-stu-id="068e1-180">String</span></span>|<span data-ttu-id="068e1-181">O endereço IPv4 do servidor DHCP para o adaptador.</span><span class="sxs-lookup"><span data-stu-id="068e1-181">The IPv4 address of the DHCP server for the adapter.</span></span>|
|<span data-ttu-id="068e1-182">ipV4DNSServerList</span><span class="sxs-lookup"><span data-stu-id="068e1-182">ipV4DNSServerList</span></span>|<span data-ttu-id="068e1-183">String collection</span><span class="sxs-lookup"><span data-stu-id="068e1-183">String collection</span></span>|<span data-ttu-id="068e1-184">Os servidores de DNS IPv4 configurados para o adaptador.</span><span class="sxs-lookup"><span data-stu-id="068e1-184">The IPv4 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="068e1-185">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="068e1-185">dnsSuffixList</span></span>|<span data-ttu-id="068e1-186">String collection</span><span class="sxs-lookup"><span data-stu-id="068e1-186">String collection</span></span>|<span data-ttu-id="068e1-187">Sufixos DNS válidos para a rede atual.</span><span class="sxs-lookup"><span data-stu-id="068e1-187">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="068e1-188">Por exemplo, seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="068e1-188">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="068e1-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="068e1-189">Response</span></span>
<span data-ttu-id="068e1-190">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="068e1-190">If successful, this method returns a `200 OK` response code and an updated [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="068e1-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="068e1-191">Example</span></span>
### <a name="request"></a><span data-ttu-id="068e1-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="068e1-192">Request</span></span>
<span data-ttu-id="068e1-193">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="068e1-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
Content-type: application/json
Content-length: 447

{
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

### <a name="response"></a><span data-ttu-id="068e1-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="068e1-194">Response</span></span>
<span data-ttu-id="068e1-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="068e1-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





