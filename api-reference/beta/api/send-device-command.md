---
title: Enviar um comando de dispositivo
description: 'Essa API permite que os recursos de projeto Roma para um dispositivo associado a uma conta da Microsoft de comando. Depois de fazer uma chamada GET em `me/devices`, passe a ID do dispositivo para emitir um comando para seu dispositivo. Dois tipos de comandos são suportados: LaunchURI e AppServices. Se você estiver usando LaunchURI, especifique os parâmetros de *tipo* e da *carga* . Para uma chamada de AppService, especifique o '
localization_priority: Normal
ms.openlocfilehash: 54349e2f43a776523614b0cd2abbc209e89305fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891984"
---
# <a name="send-device-command"></a><span data-ttu-id="c7dcc-107">Enviar um comando de dispositivo</span><span class="sxs-lookup"><span data-stu-id="c7dcc-107">Send device command</span></span>

> <span data-ttu-id="c7dcc-108">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c7dcc-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7dcc-109">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c7dcc-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c7dcc-110">Essa API permite que os recursos de projeto Roma para um dispositivo associado a uma conta da Microsoft de comando.</span><span class="sxs-lookup"><span data-stu-id="c7dcc-110">This API enables Project Rome capabilities to command a device associated with a Microsoft account.</span></span> <span data-ttu-id="c7dcc-111">Depois de fazer uma chamada GET em `me/devices`, passe a ID do dispositivo para emitir um comando para seu dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c7dcc-111">After doing a GET call on `me/devices`, pass in the ID of the device to issue a command to your device.</span></span> <span data-ttu-id="c7dcc-112">Dois tipos de comandos são suportados: LaunchURI e AppServices.</span><span class="sxs-lookup"><span data-stu-id="c7dcc-112">Two types of commands are supported: LaunchURI and AppServices.</span></span> <span data-ttu-id="c7dcc-113">Se você estiver usando LaunchURI, especifique os parâmetros de *tipo* e da *carga* .</span><span class="sxs-lookup"><span data-stu-id="c7dcc-113">If you're using LaunchURI, specify the *type* and *payload* parameters.</span></span> <span data-ttu-id="c7dcc-114">Para uma chamada de AppService, especifique o *tipo*, *carga*, *packageFamilyName*e *appServiceName* parâmetros.</span><span class="sxs-lookup"><span data-stu-id="c7dcc-114">For an AppService call, specify the *type*, *payload*, *packageFamilyName*, and *appServiceName* parameters.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7dcc-115">Permissions</span><span class="sxs-lookup"><span data-stu-id="c7dcc-115">Permissions</span></span>

<span data-ttu-id="c7dcc-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7dcc-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c7dcc-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7dcc-118">Permission type</span></span>      | <span data-ttu-id="c7dcc-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c7dcc-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7dcc-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7dcc-120">Delegated (work or school account)</span></span> | <span data-ttu-id="c7dcc-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7dcc-121">Not supported.</span></span>    |
|<span data-ttu-id="c7dcc-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7dcc-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7dcc-123">Device.Command</span><span class="sxs-lookup"><span data-stu-id="c7dcc-123">Device.Command</span></span>    |
|<span data-ttu-id="c7dcc-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7dcc-124">Application</span></span> | <span data-ttu-id="c7dcc-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7dcc-125">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7dcc-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7dcc-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST me/devices/{id}/commands
```

## <a name="request-headers"></a><span data-ttu-id="c7dcc-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7dcc-127">Request headers</span></span>


| <span data-ttu-id="c7dcc-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c7dcc-128">Header</span></span> |<span data-ttu-id="c7dcc-129">Valor</span><span class="sxs-lookup"><span data-stu-id="c7dcc-129">Value</span></span>
|:----|:------|
|<span data-ttu-id="c7dcc-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7dcc-130">Authorization</span></span>| <span data-ttu-id="c7dcc-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7dcc-p105">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="c7dcc-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c7dcc-133">Accept</span></span> | <span data-ttu-id="c7dcc-134">application/json</span><span class="sxs-lookup"><span data-stu-id="c7dcc-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7dcc-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7dcc-135">Request body</span></span>

<span data-ttu-id="c7dcc-136">No corpo da solicitação, fornece uma representação JSON das propriedades do comando.</span><span class="sxs-lookup"><span data-stu-id="c7dcc-136">In the request body, supply a JSON representation of the command properties.</span></span>

```json
{
  "type": "appService",
  "payload": "payload-JSON",
  "packageFamilyName": "packageFamilyName",
  "appServiceName": "appServiceName",
  "postbackURI": "postbackURI"
}
```

## <a name="response"></a><span data-ttu-id="c7dcc-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7dcc-137">Response</span></span>

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
## <a name="command-properties"></a><span data-ttu-id="c7dcc-138">Propriedades de comando</span><span class="sxs-lookup"><span data-stu-id="c7dcc-138">Command properties</span></span> 

|<span data-ttu-id="c7dcc-139">**Name**</span><span class="sxs-lookup"><span data-stu-id="c7dcc-139">**Name**</span></span>|<span data-ttu-id="c7dcc-140">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="c7dcc-140">**Type**</span></span>|<span data-ttu-id="c7dcc-141">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c7dcc-141">**Description**</span></span>|
|:----|:------|:------|
|<span data-ttu-id="c7dcc-142">payload</span><span class="sxs-lookup"><span data-stu-id="c7dcc-142">payload</span></span> | <span data-ttu-id="c7dcc-143">Microsoft.Graph.JSON</span><span class="sxs-lookup"><span data-stu-id="c7dcc-143">microsoft.graph.json</span></span>| <span data-ttu-id="c7dcc-144">Carga para enviar para um serviço do aplicativo ou iniciar um URI em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c7dcc-144">Payload to send to an app service or to launch a URI on a device.</span></span> |
|<span data-ttu-id="c7dcc-145">responsePayload</span><span class="sxs-lookup"><span data-stu-id="c7dcc-145">responsePayload</span></span> | <span data-ttu-id="c7dcc-146">Microsoft.Graph.JSON</span><span class="sxs-lookup"><span data-stu-id="c7dcc-146">microsoft.graph.json</span></span>| <span data-ttu-id="c7dcc-147">Carga retornado do dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="c7dcc-147">Payload returned from target device.</span></span> |
|<span data-ttu-id="c7dcc-148">postBackURI</span><span class="sxs-lookup"><span data-stu-id="c7dcc-148">postBackURI</span></span> | <span data-ttu-id="c7dcc-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7dcc-149">String</span></span> | <span data-ttu-id="c7dcc-150">URI para enviar notificações subsequentes das atualizações de volta de postagem.</span><span class="sxs-lookup"><span data-stu-id="c7dcc-150">Post back URI to send subsequent notifications of updates.</span></span> |
|<span data-ttu-id="c7dcc-151">packageFamilyName</span><span class="sxs-lookup"><span data-stu-id="c7dcc-151">packageFamilyName</span></span> | <span data-ttu-id="c7dcc-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7dcc-152">String</span></span> | <span data-ttu-id="c7dcc-153">Nome da família Windows pacote de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c7dcc-153">Windows Package Family Name of application.</span></span> |
|<span data-ttu-id="c7dcc-154">appServiceName</span><span class="sxs-lookup"><span data-stu-id="c7dcc-154">appServiceName</span></span> | <span data-ttu-id="c7dcc-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7dcc-155">String</span></span> | <span data-ttu-id="c7dcc-156">Nome do serviço de aplicativo definido pelo aplicativo de destino.</span><span class="sxs-lookup"><span data-stu-id="c7dcc-156">Name of app service defined by the target application.</span></span> <span data-ttu-id="c7dcc-157">Será necessário se lançar um serviço do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c7dcc-157">Required if launching an app service.</span></span> |
|<span data-ttu-id="c7dcc-158">type</span><span class="sxs-lookup"><span data-stu-id="c7dcc-158">type</span></span>| <span data-ttu-id="c7dcc-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7dcc-159">String</span></span> | <span data-ttu-id="c7dcc-160">LaunchURI ou AppService.</span><span class="sxs-lookup"><span data-stu-id="c7dcc-160">LaunchURI or AppService.</span></span> |
|<span data-ttu-id="c7dcc-161">id</span><span class="sxs-lookup"><span data-stu-id="c7dcc-161">id</span></span>| <span data-ttu-id="c7dcc-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7dcc-162">String</span></span> | <span data-ttu-id="c7dcc-163">A identificação de um comando que foi enviado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c7dcc-163">The ID of a command that has been sent to the device.</span></span> |
|<span data-ttu-id="c7dcc-164">actionStatus</span><span class="sxs-lookup"><span data-stu-id="c7dcc-164">actionStatus</span></span> | <span data-ttu-id="c7dcc-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7dcc-165">String</span></span> | <span data-ttu-id="c7dcc-166">O [status](get-device-command-status.md) de um comando.</span><span class="sxs-lookup"><span data-stu-id="c7dcc-166">The [status](get-device-command-status.md) of a command.</span></span> |
|<span data-ttu-id="c7dcc-167">erro</span><span class="sxs-lookup"><span data-stu-id="c7dcc-167">error</span></span>| <span data-ttu-id="c7dcc-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7dcc-168">String</span></span>| <span data-ttu-id="c7dcc-169">Quaisquer erros associados à solicitação do aplicativo de destino.</span><span class="sxs-lookup"><span data-stu-id="c7dcc-169">Any errors associated with the request from the target application.</span></span> |

## <a name="launch-uri-example"></a><span data-ttu-id="c7dcc-170">Exemplo URI de início</span><span class="sxs-lookup"><span data-stu-id="c7dcc-170">Launch URI example</span></span>

<span data-ttu-id="c7dcc-171">Aqui está um exemplo de uma solicitação de LaunchURI; ele iniciará um URI ou um aplicativo no dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="c7dcc-171">Here is an example of a LaunchURI request; it will launch a URI or an application on the target device.</span></span> <span data-ttu-id="c7dcc-172">Para iniciar um aplicativo ou um URI, emitir um POST usando a ID do dispositivo (obtido fazendo uma chamada GET em `me/devices`).</span><span class="sxs-lookup"><span data-stu-id="c7dcc-172">To launch a URI or an app, issue a POST using the ID of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="c7dcc-173">Definir os parâmetros de *tipo* para *LaunchURI* e fornecer um valor URI, tais como https://bing.com.</span><span class="sxs-lookup"><span data-stu-id="c7dcc-173">Set the *Type* parameters to *LaunchURI* and provide a URI value such as https://bing.com.</span></span>

#### <a name="request"></a><span data-ttu-id="c7dcc-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7dcc-174">Request</span></span>

<span data-ttu-id="c7dcc-175">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7dcc-175">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="c7dcc-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7dcc-176">Response</span></span> 

<span data-ttu-id="c7dcc-177">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c7dcc-177">The following is an example of the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
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


## <a name="app-service-example"></a><span data-ttu-id="c7dcc-178">Exemplo de aplicativo do serviço</span><span class="sxs-lookup"><span data-stu-id="c7dcc-178">App service example</span></span>

<span data-ttu-id="c7dcc-179">Aqui está um exemplo de uma consulta de um serviço de aplicativo em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c7dcc-179">Here is an example of querying an app service on a device.</span></span> <span data-ttu-id="c7dcc-180">Para usar um serviço de aplicativo, você deve fazer uma chamada de POSTAGEM usando a id do dispositivo (obtido fazendo uma chamada GET em `me/devices`).</span><span class="sxs-lookup"><span data-stu-id="c7dcc-180">To use an app service you must do a POST call using the id of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="c7dcc-181">Para usar o exemplo a seguir, você deve instalar o [aplicativo Roma](https://aka.ms/romanapp) no seu dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="c7dcc-181">To use the following example, you must install the [Rome app](https://aka.ms/romanapp) on your target device.</span></span>

<span data-ttu-id="c7dcc-182">Várias outras propriedades devem ser definidas na chamada.</span><span class="sxs-lookup"><span data-stu-id="c7dcc-182">Several additional properties must be set in the call.</span></span> <span data-ttu-id="c7dcc-183">*Tipo* deve ser definida como *AppService*, *AppServiceName* deve ser definida com o nome da definida no aplicativo de serviço do aplicativo, *PackageFamilyName* deve ser definida como o nome da família de pacote definido no manifesto do aplicativo e *carga* contém as chaves e valores para o serviço que você está chamando dentro do aplicativo de destino.</span><span class="sxs-lookup"><span data-stu-id="c7dcc-183">*Type* must be set to *AppService*, *AppServiceName* must be set to the name of the app service defined in the application, *PackageFamilyName* must be set to the package family name defined in the app manifest, and *Payload* holds the keys and values for the service you are calling within the target application.</span></span>

#### <a name="request"></a><span data-ttu-id="c7dcc-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7dcc-184">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="c7dcc-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7dcc-185">Response</span></span>

<span data-ttu-id="c7dcc-186">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c7dcc-186">The following is an example of the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
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
