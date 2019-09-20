---
title: Enviar comando do dispositivo
description: 'Essa API permite que os recursos do Project Roma para o comando um dispositivo associado a uma conta da Microsoft. Depois de obter uma chamada GET `me/devices`, passe a ID do dispositivo para emitir um comando para seu dispositivo. Há suporte para dois tipos de comandos: LaunchURI e AppServices. Se você estiver usando o LaunchURI, especifique os parâmetros *Type* e *Payload* . Para uma chamada serviço, especifique o '
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: f112c7d3253a0a0801b7542f492c6f3f1f675c81
ms.sourcegitcommit: 66ceeb5015ea4e92dc012cd48eee84b2bbe8e7b4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/20/2019
ms.locfileid: "37053939"
---
# <a name="send-device-command"></a><span data-ttu-id="08af7-107">Enviar comando do dispositivo</span><span class="sxs-lookup"><span data-stu-id="08af7-107">Send device command</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08af7-108">Essa API permite que os recursos do Project Roma para o comando um dispositivo associado a uma conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="08af7-108">This API enables Project Rome capabilities to command a device associated with a Microsoft account.</span></span> <span data-ttu-id="08af7-109">Depois de obter uma chamada GET `me/devices`, passe a ID do dispositivo para emitir um comando para seu dispositivo.</span><span class="sxs-lookup"><span data-stu-id="08af7-109">After doing a GET call on `me/devices`, pass in the ID of the device to issue a command to your device.</span></span> <span data-ttu-id="08af7-110">Há suporte para dois tipos de comandos: LaunchURI e AppServices.</span><span class="sxs-lookup"><span data-stu-id="08af7-110">Two types of commands are supported: LaunchURI and AppServices.</span></span> <span data-ttu-id="08af7-111">Se você estiver usando o LaunchURI, especifique os parâmetros *Type* e *Payload* .</span><span class="sxs-lookup"><span data-stu-id="08af7-111">If you're using LaunchURI, specify the *type* and *payload* parameters.</span></span> <span data-ttu-id="08af7-112">Para uma chamada serviço, especifique os parâmetros *Type*, *Payload*, *packageFamilyName*e *appServiceName* .</span><span class="sxs-lookup"><span data-stu-id="08af7-112">For an AppService call, specify the *type*, *payload*, *packageFamilyName*, and *appServiceName* parameters.</span></span>

## <a name="permissions"></a><span data-ttu-id="08af7-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="08af7-113">Permissions</span></span>

<span data-ttu-id="08af7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08af7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="08af7-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08af7-116">Permission type</span></span>      | <span data-ttu-id="08af7-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="08af7-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08af7-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08af7-118">Delegated (work or school account)</span></span> | <span data-ttu-id="08af7-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08af7-119">Not supported.</span></span>    |
|<span data-ttu-id="08af7-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08af7-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08af7-121">Device.Command</span><span class="sxs-lookup"><span data-stu-id="08af7-121">Device.Command</span></span>    |
|<span data-ttu-id="08af7-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08af7-122">Application</span></span> | <span data-ttu-id="08af7-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08af7-123">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="08af7-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08af7-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST me/devices/{id}/commands
```

## <a name="request-headers"></a><span data-ttu-id="08af7-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08af7-125">Request headers</span></span>


| <span data-ttu-id="08af7-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="08af7-126">Header</span></span> |<span data-ttu-id="08af7-127">Valor</span><span class="sxs-lookup"><span data-stu-id="08af7-127">Value</span></span>
|:----|:------|
|<span data-ttu-id="08af7-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="08af7-128">Authorization</span></span>| <span data-ttu-id="08af7-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08af7-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="08af7-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="08af7-131">Accept</span></span> | <span data-ttu-id="08af7-132">application/json</span><span class="sxs-lookup"><span data-stu-id="08af7-132">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="08af7-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08af7-133">Request body</span></span>

<span data-ttu-id="08af7-134">No corpo da solicitação, forneça uma representação JSON das propriedades do comando.</span><span class="sxs-lookup"><span data-stu-id="08af7-134">In the request body, supply a JSON representation of the command properties.</span></span>

```json
{
  "type": "appService",
  "payload": "payload-JSON",
  "packageFamilyName": "packageFamilyName",
  "appServiceName": "appServiceName",
  "postbackURI": "postbackURI"
}
```

## <a name="response"></a><span data-ttu-id="08af7-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="08af7-135">Response</span></span>

```http
HTTP/1.1 201 OK
```

```json
{
  "id": "0",
  "status": "requesting",
  "type": "appService",
  "appServiceName": "appServiceName",
  "packageFamilyName": "packageFamilyName",
  "error": "null",
  "responsePayload": "null",
  "payload": "payload-JSON",
  "permissionTicket": "null",
  "postBackUri": "postbackURI"
}
```
### <a name="command-properties"></a><span data-ttu-id="08af7-136">Propriedades de comando</span><span class="sxs-lookup"><span data-stu-id="08af7-136">Command properties</span></span> 

|<span data-ttu-id="08af7-137">**Nome**</span><span class="sxs-lookup"><span data-stu-id="08af7-137">**Name**</span></span>|<span data-ttu-id="08af7-138">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="08af7-138">**Type**</span></span>|<span data-ttu-id="08af7-139">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="08af7-139">**Description**</span></span>|
|:----|:------|:------|
|<span data-ttu-id="08af7-140">payload</span><span class="sxs-lookup"><span data-stu-id="08af7-140">payload</span></span> | <span data-ttu-id="08af7-141">Microsoft. Graph. JSON</span><span class="sxs-lookup"><span data-stu-id="08af7-141">microsoft.graph.json</span></span>| <span data-ttu-id="08af7-142">Carga a ser enviada a um serviço de aplicativo ou para iniciar um URI em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="08af7-142">Payload to send to an app service or to launch a URI on a device.</span></span> |
|<span data-ttu-id="08af7-143">responsePayload</span><span class="sxs-lookup"><span data-stu-id="08af7-143">responsePayload</span></span> | <span data-ttu-id="08af7-144">Microsoft. Graph. JSON</span><span class="sxs-lookup"><span data-stu-id="08af7-144">microsoft.graph.json</span></span>| <span data-ttu-id="08af7-145">Carga retornada do dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="08af7-145">Payload returned from target device.</span></span> |
|<span data-ttu-id="08af7-146">postBackURI</span><span class="sxs-lookup"><span data-stu-id="08af7-146">postBackURI</span></span> | <span data-ttu-id="08af7-147">String</span><span class="sxs-lookup"><span data-stu-id="08af7-147">String</span></span> | <span data-ttu-id="08af7-148">Postar URI para enviar notificações de atualizações subsequentes.</span><span class="sxs-lookup"><span data-stu-id="08af7-148">Post back URI to send subsequent notifications of updates.</span></span> |
|<span data-ttu-id="08af7-149">packageFamilyName</span><span class="sxs-lookup"><span data-stu-id="08af7-149">packageFamilyName</span></span> | <span data-ttu-id="08af7-150">String</span><span class="sxs-lookup"><span data-stu-id="08af7-150">String</span></span> | <span data-ttu-id="08af7-151">Nome do aplicativo da família de pacote do Windows.</span><span class="sxs-lookup"><span data-stu-id="08af7-151">Windows Package Family Name of application.</span></span> |
|<span data-ttu-id="08af7-152">appServiceName</span><span class="sxs-lookup"><span data-stu-id="08af7-152">appServiceName</span></span> | <span data-ttu-id="08af7-153">String</span><span class="sxs-lookup"><span data-stu-id="08af7-153">String</span></span> | <span data-ttu-id="08af7-154">Nome do serviço de aplicativo definido pelo aplicativo de destino.</span><span class="sxs-lookup"><span data-stu-id="08af7-154">Name of app service defined by the target application.</span></span> <span data-ttu-id="08af7-155">Necessário se iniciar um serviço de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="08af7-155">Required if launching an app service.</span></span> |
|<span data-ttu-id="08af7-156">type</span><span class="sxs-lookup"><span data-stu-id="08af7-156">type</span></span>| <span data-ttu-id="08af7-157">String</span><span class="sxs-lookup"><span data-stu-id="08af7-157">String</span></span> | <span data-ttu-id="08af7-158">LaunchURI ou serviço.</span><span class="sxs-lookup"><span data-stu-id="08af7-158">LaunchURI or AppService.</span></span> |
|<span data-ttu-id="08af7-159">id</span><span class="sxs-lookup"><span data-stu-id="08af7-159">id</span></span>| <span data-ttu-id="08af7-160">String</span><span class="sxs-lookup"><span data-stu-id="08af7-160">String</span></span> | <span data-ttu-id="08af7-161">A ID de um comando que foi enviado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="08af7-161">The ID of a command that has been sent to the device.</span></span> |
|<span data-ttu-id="08af7-162">actionStatus</span><span class="sxs-lookup"><span data-stu-id="08af7-162">actionStatus</span></span> | <span data-ttu-id="08af7-163">String</span><span class="sxs-lookup"><span data-stu-id="08af7-163">String</span></span> | <span data-ttu-id="08af7-164">O [status](get-device-command-status.md) de um comando.</span><span class="sxs-lookup"><span data-stu-id="08af7-164">The [status](get-device-command-status.md) of a command.</span></span> |
|<span data-ttu-id="08af7-165">erro</span><span class="sxs-lookup"><span data-stu-id="08af7-165">error</span></span>| <span data-ttu-id="08af7-166">String</span><span class="sxs-lookup"><span data-stu-id="08af7-166">String</span></span>| <span data-ttu-id="08af7-167">Quaisquer erros associados à solicitação do aplicativo de destino.</span><span class="sxs-lookup"><span data-stu-id="08af7-167">Any errors associated with the request from the target application.</span></span> |

## <a name="examples"></a><span data-ttu-id="08af7-168">Exemplos</span><span class="sxs-lookup"><span data-stu-id="08af7-168">Examples</span></span>

### <a name="example-1-launch-uri"></a><span data-ttu-id="08af7-169">Exemplo 1: URI de lançamento</span><span class="sxs-lookup"><span data-stu-id="08af7-169">Example 1: Launch URI</span></span> 

<span data-ttu-id="08af7-170">Este é um exemplo de uma solicitação LaunchURI; ele iniciará um URI ou um aplicativo no dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="08af7-170">The following is an example of a LaunchURI request; it will launch a URI or an application on the target device.</span></span> <span data-ttu-id="08af7-171">Para iniciar um URI ou um aplicativo, emita uma POSTAgem usando a ID do dispositivo (obtido de uma chamada GET ativada `me/devices`).</span><span class="sxs-lookup"><span data-stu-id="08af7-171">To launch a URI or an app, issue a POST using the ID of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="08af7-172">Defina os parâmetros de *tipo* como *LaunchURI* e forneça um valor de URI https://bing.comcomo.</span><span class="sxs-lookup"><span data-stu-id="08af7-172">Set the *Type* parameters to *LaunchURI* and provide a URI value such as https://bing.com.</span></span>

#### <a name="request"></a><span data-ttu-id="08af7-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08af7-173">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_command"
} -->

```http

POST me/devices/{id}/commands
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8

{ "type" : "LaunchUri", "payload" : {"uri":"https://bing.com"}}

```
#### <a name="response"></a><span data-ttu-id="08af7-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="08af7-174">Response</span></span> 

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.command",
  "isCollection": true
} -->

```http
HTTP/1.1 201 OK

{
  "id": "0158355AD4D680CC4E2994CC009EFFD7337D1B...",
  "status": "requesting",
  "type": null,
  "appServiceName": null,
  "packageFamilyName": null,
  "error": null,
  "permissionTicket": null,
  "postBackUri": null,
  "payload": {
    "uri": "https://bing.com"
  }
}

```


### <a name="example-2-app-service"></a><span data-ttu-id="08af7-175">Exemplo 2: serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="08af7-175">Example 2: App service</span></span>

<span data-ttu-id="08af7-176">O exemplo a seguir mostra como consultar um serviço de aplicativo em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="08af7-176">The following example shows how to query an app service on a device.</span></span> <span data-ttu-id="08af7-177">Para usar um serviço de aplicativo, você deve fazer uma chamada POST usando a ID do dispositivo (obtido de uma chamada GET ativada `me/devices`).</span><span class="sxs-lookup"><span data-stu-id="08af7-177">To use an app service, you must do a POST call using the ID of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="08af7-178">Para usar o exemplo a seguir, você deve instalar o [aplicativo Roma](https://aka.ms/romanapp) no seu dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="08af7-178">To use the following example, you must install the [Rome app](https://aka.ms/romanapp) on your target device.</span></span>

<span data-ttu-id="08af7-179">Várias propriedades adicionais devem ser definidas na chamada.</span><span class="sxs-lookup"><span data-stu-id="08af7-179">Several additional properties must be set in the call.</span></span> <span data-ttu-id="08af7-180">O *tipo* deve ser definido *como serviço*, *AppServiceName* deve ser definido como o nome do serviço de aplicativo definido no aplicativo, *PackageFamilyName* deve ser definido como o nome da família do pacote definido no manifesto do aplicativo e *carga* contém as chaves e os valores para o serviço que você está chamando no aplicativo de destino.</span><span class="sxs-lookup"><span data-stu-id="08af7-180">*Type* must be set to *AppService*, *AppServiceName* must be set to the name of the app service defined in the application, *PackageFamilyName* must be set to the package family name defined in the app manifest, and *Payload* holds the keys and values for the service you are calling within the target application.</span></span>

#### <a name="request"></a><span data-ttu-id="08af7-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08af7-181">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_command_2"
} -->

```http

POST me/devices/{id}/commands
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8

{
  "type" : "AppService",
  "appServiceName" : "com.microsoft.test.cdppingpongservice",
  "packageFamilyName" : "5085ShawnHenry.RomanTestApp_jsjw7knzsgcce",
  "payload" : {
    "Type":"Toast","Title":"Hello","Subtitle":"World!"}
  }
```

#### <a name="response"></a><span data-ttu-id="08af7-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="08af7-182">Response</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.command",
  "isCollection": true
} -->

```http
HTTP/1.1 201 OK

{
  "id": "0158355AD4D680CC4E2994CC009EFFD7EADA8307E96FF1C8D19B..",
  "status": "requesting",
  "type": null,
  "appServiceName": "com.microsoft.randomnumbergenerator",
  "packageFamilyName": "Microsoft.SDKSamples.AppServicesProvider.CS_8wekyb3d8bbwe",
  "error": null,
  "permissionTicket": null,
  "postBackUri": null,
  "payload": {
    "Type": "Toast",
    "Title": "Hello",
    "Subtitle": "World!"
  }
}
```
