---
title: Atualizar cartToClassAssociation
description: Atualiza as propriedades de um objeto cartToClassAssociation.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 497038aad85c9fa9df2b29184a729b46af42602a
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39954479"
---
# <a name="update-carttoclassassociation"></a><span data-ttu-id="abda3-103">Atualizar cartToClassAssociation</span><span class="sxs-lookup"><span data-stu-id="abda3-103">Update cartToClassAssociation</span></span>

> <span data-ttu-id="abda3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="abda3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abda3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="abda3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abda3-106">Atualiza as propriedades de um objeto [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) .</span><span class="sxs-lookup"><span data-stu-id="abda3-106">Update the properties of a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="abda3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="abda3-107">Prerequisites</span></span>
<span data-ttu-id="abda3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abda3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abda3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="abda3-110">Permission type</span></span>|<span data-ttu-id="abda3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="abda3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abda3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="abda3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="abda3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abda3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="abda3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="abda3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abda3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abda3-115">Not supported.</span></span>|
|<span data-ttu-id="abda3-116">Application</span><span class="sxs-lookup"><span data-stu-id="abda3-116">Application</span></span>|<span data-ttu-id="abda3-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abda3-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="abda3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="abda3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
```

## <a name="request-headers"></a><span data-ttu-id="abda3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="abda3-119">Request headers</span></span>
|<span data-ttu-id="abda3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="abda3-120">Header</span></span>|<span data-ttu-id="abda3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="abda3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abda3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="abda3-122">Authorization</span></span>|<span data-ttu-id="abda3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="abda3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abda3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="abda3-124">Accept</span></span>|<span data-ttu-id="abda3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="abda3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abda3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="abda3-126">Request body</span></span>
<span data-ttu-id="abda3-127">No corpo da solicitação, forneça uma representação JSON do objeto [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) .</span><span class="sxs-lookup"><span data-stu-id="abda3-127">In the request body, supply a JSON representation for the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

<span data-ttu-id="abda3-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).</span><span class="sxs-lookup"><span data-stu-id="abda3-128">The following table shows the properties that are required when you create the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).</span></span>

|<span data-ttu-id="abda3-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="abda3-129">Property</span></span>|<span data-ttu-id="abda3-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="abda3-130">Type</span></span>|<span data-ttu-id="abda3-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="abda3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abda3-132">id</span><span class="sxs-lookup"><span data-stu-id="abda3-132">id</span></span>|<span data-ttu-id="abda3-133">String</span><span class="sxs-lookup"><span data-stu-id="abda3-133">String</span></span>|<span data-ttu-id="abda3-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="abda3-134">Key of the entity.</span></span>|
|<span data-ttu-id="abda3-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="abda3-135">createdDateTime</span></span>|<span data-ttu-id="abda3-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abda3-136">DateTimeOffset</span></span>|<span data-ttu-id="abda3-137">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="abda3-137">DateTime the object was created.</span></span>|
|<span data-ttu-id="abda3-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="abda3-138">lastModifiedDateTime</span></span>|<span data-ttu-id="abda3-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abda3-139">DateTimeOffset</span></span>|<span data-ttu-id="abda3-140">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="abda3-140">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="abda3-141">versão</span><span class="sxs-lookup"><span data-stu-id="abda3-141">version</span></span>|<span data-ttu-id="abda3-142">Int32</span><span class="sxs-lookup"><span data-stu-id="abda3-142">Int32</span></span>|<span data-ttu-id="abda3-143">Versão do CartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="abda3-143">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="abda3-144">displayName</span><span class="sxs-lookup"><span data-stu-id="abda3-144">displayName</span></span>|<span data-ttu-id="abda3-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="abda3-145">String</span></span>|<span data-ttu-id="abda3-146">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="abda3-146">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="abda3-147">description</span><span class="sxs-lookup"><span data-stu-id="abda3-147">description</span></span>|<span data-ttu-id="abda3-148">String</span><span class="sxs-lookup"><span data-stu-id="abda3-148">String</span></span>|<span data-ttu-id="abda3-149">Descrição fornecida pelo administrador do CartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="abda3-149">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="abda3-150">deviceCartIds</span><span class="sxs-lookup"><span data-stu-id="abda3-150">deviceCartIds</span></span>|<span data-ttu-id="abda3-151">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="abda3-151">String collection</span></span>|<span data-ttu-id="abda3-152">Identificadores de carrinhos de dispositivos a serem associados às classes.</span><span class="sxs-lookup"><span data-stu-id="abda3-152">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="abda3-153">classroomIds</span><span class="sxs-lookup"><span data-stu-id="abda3-153">classroomIds</span></span>|<span data-ttu-id="abda3-154">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="abda3-154">String collection</span></span>|<span data-ttu-id="abda3-155">Identificadores de salas de aula a serem associadas a carrinhos de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="abda3-155">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="abda3-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="abda3-156">Response</span></span>
<span data-ttu-id="abda3-157">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="abda3-157">If successful, this method returns a `200 OK` response code and an updated [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abda3-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="abda3-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="abda3-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="abda3-159">Request</span></span>
<span data-ttu-id="abda3-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="abda3-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="abda3-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="abda3-161">Response</span></span>
<span data-ttu-id="abda3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="abda3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





