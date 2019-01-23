---
title: Criar officeClientConfigurationAssignment
description: Adicione um grupo-alvo a uma política existente.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c1f09ba2dfabf85501120cb2099373e5664deb08
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425194"
---
# <a name="create-officeclientconfigurationassignment"></a><span data-ttu-id="57504-103">Criar officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="57504-103">Create officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="57504-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="57504-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="57504-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="57504-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="57504-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="57504-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57504-107">Adicione um grupo-alvo a uma política existente.</span><span class="sxs-lookup"><span data-stu-id="57504-107">Add a target group to an existing policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57504-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="57504-108">Prerequisites</span></span>
<span data-ttu-id="57504-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57504-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57504-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57504-111">Permission type</span></span>|<span data-ttu-id="57504-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="57504-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57504-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57504-113">Delegated (work or school account)</span></span>|<span data-ttu-id="57504-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57504-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="57504-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57504-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57504-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57504-116">Not supported.</span></span>|
|<span data-ttu-id="57504-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57504-117">Application</span></span>|<span data-ttu-id="57504-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57504-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57504-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57504-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{key}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="57504-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57504-120">Request headers</span></span>
|<span data-ttu-id="57504-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="57504-121">Header</span></span>|<span data-ttu-id="57504-122">Valor</span><span class="sxs-lookup"><span data-stu-id="57504-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57504-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="57504-123">Authorization</span></span>|<span data-ttu-id="57504-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57504-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57504-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="57504-125">Accept</span></span>|<span data-ttu-id="57504-126">application/json</span><span class="sxs-lookup"><span data-stu-id="57504-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57504-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57504-127">Request body</span></span>
<span data-ttu-id="57504-128">No corpo da solicitação, fornece uma representação JSON para o objeto officeClientConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="57504-128">In the request body, supply a JSON representation for the officeClientConfigurationAssignment object.</span></span>

<span data-ttu-id="57504-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o officeClientConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="57504-129">The following table shows the properties that are required when you create the officeClientConfigurationAssignment.</span></span>

|<span data-ttu-id="57504-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57504-130">Property</span></span>|<span data-ttu-id="57504-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="57504-131">Type</span></span>|<span data-ttu-id="57504-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="57504-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57504-133">id</span><span class="sxs-lookup"><span data-stu-id="57504-133">id</span></span>|<span data-ttu-id="57504-134">String</span><span class="sxs-lookup"><span data-stu-id="57504-134">String</span></span>|<span data-ttu-id="57504-135">ID do OfficeConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="57504-135">Id of the OfficeConfigurationAssignment.</span></span>|
|<span data-ttu-id="57504-136">destino</span><span class="sxs-lookup"><span data-stu-id="57504-136">target</span></span>|[<span data-ttu-id="57504-137">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="57504-137">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="57504-138">A atribuição de destino definida pelo administrador a.</span><span class="sxs-lookup"><span data-stu-id="57504-138">The target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="57504-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="57504-139">Response</span></span>
<span data-ttu-id="57504-140">Se tiver êxito, este método retornará um `200 Created` código de resposta e um objeto [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="57504-140">If successful, this method returns a `200 Created` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57504-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="57504-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="57504-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57504-142">Request</span></span>
<span data-ttu-id="57504-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="57504-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="57504-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="57504-144">Response</span></span>
<span data-ttu-id="57504-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="57504-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "id": "804730f3-30f3-8047-f330-4780f3304780",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```



