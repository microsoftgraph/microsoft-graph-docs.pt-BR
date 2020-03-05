---
title: Atualizar cartToClassAssociation
description: Atualiza as propriedades de um objeto cartToClassAssociation.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 35b53c2d5bdb00b35b3b351ad83ff513ae950cec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42443304"
---
# <a name="update-carttoclassassociation"></a><span data-ttu-id="d4568-103">Atualizar cartToClassAssociation</span><span class="sxs-lookup"><span data-stu-id="d4568-103">Update cartToClassAssociation</span></span>

<span data-ttu-id="d4568-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d4568-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4568-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d4568-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4568-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d4568-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4568-107">Atualiza as propriedades de um objeto [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) .</span><span class="sxs-lookup"><span data-stu-id="d4568-107">Update the properties of a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4568-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d4568-108">Prerequisites</span></span>
<span data-ttu-id="d4568-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4568-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4568-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4568-111">Permission type</span></span>|<span data-ttu-id="d4568-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d4568-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4568-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4568-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4568-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4568-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d4568-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4568-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4568-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4568-116">Not supported.</span></span>|
|<span data-ttu-id="d4568-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4568-117">Application</span></span>|<span data-ttu-id="d4568-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4568-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4568-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4568-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
```

## <a name="request-headers"></a><span data-ttu-id="d4568-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4568-120">Request headers</span></span>
|<span data-ttu-id="d4568-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d4568-121">Header</span></span>|<span data-ttu-id="d4568-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d4568-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4568-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4568-123">Authorization</span></span>|<span data-ttu-id="d4568-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4568-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4568-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d4568-125">Accept</span></span>|<span data-ttu-id="d4568-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4568-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4568-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4568-127">Request body</span></span>
<span data-ttu-id="d4568-128">No corpo da solicitação, forneça uma representação JSON do objeto [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) .</span><span class="sxs-lookup"><span data-stu-id="d4568-128">In the request body, supply a JSON representation for the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

<span data-ttu-id="d4568-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).</span><span class="sxs-lookup"><span data-stu-id="d4568-129">The following table shows the properties that are required when you create the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).</span></span>

|<span data-ttu-id="d4568-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4568-130">Property</span></span>|<span data-ttu-id="d4568-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4568-131">Type</span></span>|<span data-ttu-id="d4568-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4568-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4568-133">id</span><span class="sxs-lookup"><span data-stu-id="d4568-133">id</span></span>|<span data-ttu-id="d4568-134">String</span><span class="sxs-lookup"><span data-stu-id="d4568-134">String</span></span>|<span data-ttu-id="d4568-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d4568-135">Key of the entity.</span></span>|
|<span data-ttu-id="d4568-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d4568-136">createdDateTime</span></span>|<span data-ttu-id="d4568-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4568-137">DateTimeOffset</span></span>|<span data-ttu-id="d4568-138">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d4568-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="d4568-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4568-139">lastModifiedDateTime</span></span>|<span data-ttu-id="d4568-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4568-140">DateTimeOffset</span></span>|<span data-ttu-id="d4568-141">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d4568-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="d4568-142">versão</span><span class="sxs-lookup"><span data-stu-id="d4568-142">version</span></span>|<span data-ttu-id="d4568-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d4568-143">Int32</span></span>|<span data-ttu-id="d4568-144">Versão do CartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="d4568-144">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="d4568-145">displayName</span><span class="sxs-lookup"><span data-stu-id="d4568-145">displayName</span></span>|<span data-ttu-id="d4568-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4568-146">String</span></span>|<span data-ttu-id="d4568-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d4568-147">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="d4568-148">description</span><span class="sxs-lookup"><span data-stu-id="d4568-148">description</span></span>|<span data-ttu-id="d4568-149">String</span><span class="sxs-lookup"><span data-stu-id="d4568-149">String</span></span>|<span data-ttu-id="d4568-150">Descrição fornecida pelo administrador do CartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="d4568-150">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="d4568-151">deviceCartIds</span><span class="sxs-lookup"><span data-stu-id="d4568-151">deviceCartIds</span></span>|<span data-ttu-id="d4568-152">String collection</span><span class="sxs-lookup"><span data-stu-id="d4568-152">String collection</span></span>|<span data-ttu-id="d4568-153">Identificadores de carrinhos de dispositivos a serem associados às classes.</span><span class="sxs-lookup"><span data-stu-id="d4568-153">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="d4568-154">classroomIds</span><span class="sxs-lookup"><span data-stu-id="d4568-154">classroomIds</span></span>|<span data-ttu-id="d4568-155">String collection</span><span class="sxs-lookup"><span data-stu-id="d4568-155">String collection</span></span>|<span data-ttu-id="d4568-156">Identificadores de salas de aula a serem associadas a carrinhos de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="d4568-156">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="d4568-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4568-157">Response</span></span>
<span data-ttu-id="d4568-158">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4568-158">If successful, this method returns a `200 OK` response code and an updated [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4568-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4568-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4568-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4568-160">Request</span></span>
<span data-ttu-id="d4568-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4568-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
Content-type: application/json
Content-length: 271

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "deviceCartIds": [
    "Device Cart Ids value"
  ],
  "classroomIds": [
    "Classroom Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="d4568-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4568-162">Response</span></span>
<span data-ttu-id="d4568-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d4568-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 443

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "id": "9bdc58dd-58dd-9bdc-dd58-dc9bdd58dc9b",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "deviceCartIds": [
    "Device Cart Ids value"
  ],
  "classroomIds": [
    "Classroom Ids value"
  ]
}
```





