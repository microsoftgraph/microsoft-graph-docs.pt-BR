---
title: Criar networkIPv4ConfigurationManagementCondition
description: Crie um novo objeto de networkIPv4ConfigurationManagementCondition.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 385e24e7b20624a82f7744957668d7a36280af11
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394751"
---
# <a name="create-networkipv4configurationmanagementcondition"></a><span data-ttu-id="c1bd1-103">Criar networkIPv4ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="c1bd1-103">Create networkIPv4ConfigurationManagementCondition</span></span>

> <span data-ttu-id="c1bd1-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="c1bd1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c1bd1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c1bd1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1bd1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="c1bd1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1bd1-107">Crie um novo objeto de [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="c1bd1-107">Create a new [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1bd1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c1bd1-108">Prerequisites</span></span>
<span data-ttu-id="c1bd1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c1bd1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c1bd1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c1bd1-111">Permission type</span></span>|<span data-ttu-id="c1bd1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c1bd1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1bd1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c1bd1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c1bd1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1bd1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c1bd1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c1bd1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1bd1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1bd1-116">Not supported.</span></span>|
|<span data-ttu-id="c1bd1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c1bd1-117">Application</span></span>|<span data-ttu-id="c1bd1-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1bd1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1bd1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c1bd1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="c1bd1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c1bd1-120">Request headers</span></span>
|<span data-ttu-id="c1bd1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c1bd1-121">Header</span></span>|<span data-ttu-id="c1bd1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c1bd1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1bd1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c1bd1-123">Authorization</span></span>|<span data-ttu-id="c1bd1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1bd1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1bd1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c1bd1-125">Accept</span></span>|<span data-ttu-id="c1bd1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c1bd1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1bd1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c1bd1-127">Request body</span></span>
<span data-ttu-id="c1bd1-128">No corpo da solicitação, fornece uma representação JSON para o objeto networkIPv4ConfigurationManagementCondition.</span><span class="sxs-lookup"><span data-stu-id="c1bd1-128">In the request body, supply a JSON representation for the networkIPv4ConfigurationManagementCondition object.</span></span>

<span data-ttu-id="c1bd1-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o networkIPv4ConfigurationManagementCondition.</span><span class="sxs-lookup"><span data-stu-id="c1bd1-129">The following table shows the properties that are required when you create the networkIPv4ConfigurationManagementCondition.</span></span>

|<span data-ttu-id="c1bd1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1bd1-130">Property</span></span>|<span data-ttu-id="c1bd1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1bd1-131">Type</span></span>|<span data-ttu-id="c1bd1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1bd1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1bd1-133">id</span><span class="sxs-lookup"><span data-stu-id="c1bd1-133">id</span></span>|<span data-ttu-id="c1bd1-134">String</span><span class="sxs-lookup"><span data-stu-id="c1bd1-134">String</span></span>|<span data-ttu-id="c1bd1-135">Identificador exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="c1bd1-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="c1bd1-136">Valor atribuído quando criado gerado pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="c1bd1-136">System generated value assigned when created.</span></span> <span data-ttu-id="c1bd1-137">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="c1bd1-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="c1bd1-138">nome exclusivo</span><span class="sxs-lookup"><span data-stu-id="c1bd1-138">uniqueName</span></span>|<span data-ttu-id="c1bd1-139">String</span><span class="sxs-lookup"><span data-stu-id="c1bd1-139">String</span></span>|<span data-ttu-id="c1bd1-140">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="c1bd1-140">Unique name for the management condition.</span></span> <span data-ttu-id="c1bd1-141">Usadas nas expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="c1bd1-141">Used in management condition expressions.</span></span> <span data-ttu-id="c1bd1-142">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="c1bd1-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="c1bd1-143">displayName</span><span class="sxs-lookup"><span data-stu-id="c1bd1-143">displayName</span></span>|<span data-ttu-id="c1bd1-144">String</span><span class="sxs-lookup"><span data-stu-id="c1bd1-144">String</span></span>|<span data-ttu-id="c1bd1-145">O nome definido admin da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="c1bd1-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="c1bd1-146">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="c1bd1-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="c1bd1-147">description</span><span class="sxs-lookup"><span data-stu-id="c1bd1-147">description</span></span>|<span data-ttu-id="c1bd1-148">String</span><span class="sxs-lookup"><span data-stu-id="c1bd1-148">String</span></span>|<span data-ttu-id="c1bd1-149">O administrador definidos descrição da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="c1bd1-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="c1bd1-150">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="c1bd1-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="c1bd1-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c1bd1-151">createdDateTime</span></span>|<span data-ttu-id="c1bd1-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1bd1-152">DateTimeOffset</span></span>|<span data-ttu-id="c1bd1-153">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="c1bd1-153">The time the management condition was created.</span></span> <span data-ttu-id="c1bd1-154">Lado de serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="c1bd1-154">Generated service side.</span></span> <span data-ttu-id="c1bd1-155">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="c1bd1-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="c1bd1-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1bd1-156">modifiedDateTime</span></span>|<span data-ttu-id="c1bd1-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1bd1-157">DateTimeOffset</span></span>|<span data-ttu-id="c1bd1-158">A hora que da última modificação a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="c1bd1-158">The time the management condition was last modified.</span></span> <span data-ttu-id="c1bd1-159">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="c1bd1-159">Updated service side.</span></span> <span data-ttu-id="c1bd1-160">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="c1bd1-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="c1bd1-161">eTag</span><span class="sxs-lookup"><span data-stu-id="c1bd1-161">eTag</span></span>|<span data-ttu-id="c1bd1-162">String</span><span class="sxs-lookup"><span data-stu-id="c1bd1-162">String</span></span>|<span data-ttu-id="c1bd1-163">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="c1bd1-163">ETag of the management condition.</span></span> <span data-ttu-id="c1bd1-164">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="c1bd1-164">Updated service side.</span></span> <span data-ttu-id="c1bd1-165">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="c1bd1-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="c1bd1-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="c1bd1-166">applicablePlatforms</span></span>|<span data-ttu-id="c1bd1-167">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="c1bd1-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="c1bd1-168">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="c1bd1-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="c1bd1-169">Herdada do [managementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="c1bd1-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="c1bd1-170">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="c1bd1-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="c1bd1-171">ipV4Prefix</span><span class="sxs-lookup"><span data-stu-id="c1bd1-171">ipV4Prefix</span></span>|<span data-ttu-id="c1bd1-172">String</span><span class="sxs-lookup"><span data-stu-id="c1bd1-172">String</span></span>|<span data-ttu-id="c1bd1-173">A sub-rede IPv4 seja conectada.</span><span class="sxs-lookup"><span data-stu-id="c1bd1-173">The IPv4 subnet to be connected to.</span></span> <span data-ttu-id="c1bd1-174">Por exemplo, 10.0.0.0/8</span><span class="sxs-lookup"><span data-stu-id="c1bd1-174">e.g. 10.0.0.0/8</span></span>|
|<span data-ttu-id="c1bd1-175">ipV4Gateway</span><span class="sxs-lookup"><span data-stu-id="c1bd1-175">ipV4Gateway</span></span>|<span data-ttu-id="c1bd1-176">String</span><span class="sxs-lookup"><span data-stu-id="c1bd1-176">String</span></span>|<span data-ttu-id="c1bd1-177">O endereço de gateway IPv4.</span><span class="sxs-lookup"><span data-stu-id="c1bd1-177">The IPv4 gateway address.</span></span> <span data-ttu-id="c1bd1-178">Por exemplo, 10.0.0.0</span><span class="sxs-lookup"><span data-stu-id="c1bd1-178">e.g. 10.0.0.0</span></span>|
|<span data-ttu-id="c1bd1-179">ipV4DHCPServer</span><span class="sxs-lookup"><span data-stu-id="c1bd1-179">ipV4DHCPServer</span></span>|<span data-ttu-id="c1bd1-180">String</span><span class="sxs-lookup"><span data-stu-id="c1bd1-180">String</span></span>|<span data-ttu-id="c1bd1-181">O endereço IPv4 do servidor DHCP para o adaptador.</span><span class="sxs-lookup"><span data-stu-id="c1bd1-181">The IPv4 address of the DHCP server for the adapter.</span></span>|
|<span data-ttu-id="c1bd1-182">ipV4DNSServerList</span><span class="sxs-lookup"><span data-stu-id="c1bd1-182">ipV4DNSServerList</span></span>|<span data-ttu-id="c1bd1-183">String collection</span><span class="sxs-lookup"><span data-stu-id="c1bd1-183">String collection</span></span>|<span data-ttu-id="c1bd1-184">Os servidores de DNS IPv4 configurados para o adaptador.</span><span class="sxs-lookup"><span data-stu-id="c1bd1-184">The IPv4 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="c1bd1-185">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="c1bd1-185">dnsSuffixList</span></span>|<span data-ttu-id="c1bd1-186">String collection</span><span class="sxs-lookup"><span data-stu-id="c1bd1-186">String collection</span></span>|<span data-ttu-id="c1bd1-187">Sufixos DNS válidos para a rede atual.</span><span class="sxs-lookup"><span data-stu-id="c1bd1-187">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="c1bd1-188">Por exemplo, seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="c1bd1-188">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="c1bd1-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1bd1-189">Response</span></span>
<span data-ttu-id="c1bd1-190">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c1bd1-190">If successful, this method returns a `201 Created` response code and a [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1bd1-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c1bd1-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1bd1-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c1bd1-192">Request</span></span>
<span data-ttu-id="c1bd1-193">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c1bd1-193">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c1bd1-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1bd1-194">Response</span></span>
<span data-ttu-id="c1bd1-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c1bd1-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




