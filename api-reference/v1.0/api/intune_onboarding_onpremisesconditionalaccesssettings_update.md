# <a name="update-onpremisesconditionalaccesssettings"></a>Atualizar onPremisesConditionalAccessSettings

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Atualizar as propriedades de um objeto [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md).
## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/conditionalAccessSettings
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|Token&gt; de portador obrigatório.&lt;|
|Aceitar|aplicativo/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md).

A tabela a seguir mostra as propriedades obrigatórias ao criar [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Ainda não documentado|
|enabled|Booliano|Indica se o acesso condicional local está habilitado para esta organização|
|includedGroups|Coleção de GUIDs|Grupos de usuários que serão direcionados pelo acesso condicional local. Todos os usuários nesses grupos deverão ter dispositivos móveis gerenciados e compatíveis com o acesso a email.|
|excludedGroups|Coleção de GUIDs|Grupos de usuários que estarão isentos ao acesso condicional local. Todos os usuários desses grupos ficarão isentos da política de acesso condicional.|
|overrideDefaultRule|Booliano|Substitui as regras de acesso padrão ao permitir a um dispositivo que seja concedida a garantia de acesso.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/conditionalAccessSettings
Content-type: application/json
Content-length: 195

{
  "enabled": true,
  "includedGroups": [
    "<Unknown Primitive Type Edm.Guid>"
  ],
  "excludedGroups": [
    "<Unknown Primitive Type Edm.Guid>"
  ],
  "overrideDefaultRule": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 318

{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "a0efde21-de21-a0ef-21de-efa021deefa0",
  "enabled": true,
  "includedGroups": [
    "String"
  ],
  "excludedGroups": [
    "String"
  ],
  "overrideDefaultRule": true
}
```








