# <a name="update-androidforworkappconfigurationschema"></a><span data-ttu-id="d40b1-101">Atualizar androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="d40b1-101">Update androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="d40b1-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d40b1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d40b1-103">Atualizar as propriedades de um objeto [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="d40b1-103">Update the properties of a [calendar](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d40b1-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d40b1-104">Prerequisites</span></span>
<span data-ttu-id="d40b1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d40b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d40b1-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d40b1-107">Permission type</span></span>|<span data-ttu-id="d40b1-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d40b1-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d40b1-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d40b1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d40b1-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d40b1-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d40b1-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d40b1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d40b1-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d40b1-112">Not supported.</span></span>|
|<span data-ttu-id="d40b1-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d40b1-113">Application</span></span>|<span data-ttu-id="d40b1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d40b1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d40b1-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d40b1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="d40b1-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d40b1-116">Request headers</span></span>
|<span data-ttu-id="d40b1-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d40b1-117">Header</span></span>|<span data-ttu-id="d40b1-118">Valor</span><span class="sxs-lookup"><span data-stu-id="d40b1-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d40b1-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="d40b1-119">Authorization</span></span>|<span data-ttu-id="d40b1-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d40b1-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d40b1-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d40b1-121">Accept</span></span>|<span data-ttu-id="d40b1-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d40b1-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d40b1-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d40b1-123">Request body</span></span>
<span data-ttu-id="d40b1-124">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="d40b1-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) object.</span></span>

<span data-ttu-id="d40b1-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="d40b1-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="d40b1-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d40b1-126">Property</span></span>|<span data-ttu-id="d40b1-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="d40b1-127">Type</span></span>|<span data-ttu-id="d40b1-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="d40b1-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d40b1-129">id</span><span class="sxs-lookup"><span data-stu-id="d40b1-129">id</span></span>|<span data-ttu-id="d40b1-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d40b1-130">String</span></span>|<span data-ttu-id="d40b1-131">A chave da entidade ao qual o nome do pacote Android para o aplicativo cujo esquema corresponde a</span><span class="sxs-lookup"><span data-stu-id="d40b1-131">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="d40b1-132">exampleJson</span><span class="sxs-lookup"><span data-stu-id="d40b1-132">exampleJson</span></span>|<span data-ttu-id="d40b1-133">Binária</span><span class="sxs-lookup"><span data-stu-id="d40b1-133">Binary</span></span>|<span data-ttu-id="d40b1-134">A matriz de bytes codificados de UTF8 que contém exemplo de cadeia JSON em conformidade com esse esquema que demonstra como definir a configuração para esse aplicativo</span><span class="sxs-lookup"><span data-stu-id="d40b1-134">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="d40b1-135">schemaItems</span><span class="sxs-lookup"><span data-stu-id="d40b1-135">schemaItems</span></span>|<span data-ttu-id="d40b1-136">Coleção [androidForWorkAppConfigurationSchemaItem](../resources/intune_androidforwork_androidforworkappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="d40b1-136">[androidForWorkAppConfigurationSchemaItem](../resources/intune_androidforwork_androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="d40b1-137">Coleção de itens que representa uma opção de configuração nomeada no esquema</span><span class="sxs-lookup"><span data-stu-id="d40b1-137">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="d40b1-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d40b1-138">Response</span></span>
<span data-ttu-id="d40b1-139">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d40b1-139">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d40b1-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d40b1-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="d40b1-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d40b1-141">Request</span></span>
<span data-ttu-id="d40b1-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d40b1-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
Content-type: application/json
Content-length: 720

{
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
      "schemaItemKey": "Schema Item Key value",
      "displayName": "Display Name value",
      "description": "Description value",
      "defaultBoolValue": true,
      "defaultIntValue": 15,
      "defaultStringValue": "Default String Value value",
      "defaultStringArrayValue": [
        "Default String Array Value value"
      ],
      "dataType": "integer",
      "selections": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="d40b1-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d40b1-143">Response</span></span>
<span data-ttu-id="d40b1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d40b1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 844

{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
  "id": "c1230dc6-0dc6-c123-c60d-23c1c60d23c1",
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
      "schemaItemKey": "Schema Item Key value",
      "displayName": "Display Name value",
      "description": "Description value",
      "defaultBoolValue": true,
      "defaultIntValue": 15,
      "defaultStringValue": "Default String Value value",
      "defaultStringArrayValue": [
        "Default String Array Value value"
      ],
      "dataType": "integer",
      "selections": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```



