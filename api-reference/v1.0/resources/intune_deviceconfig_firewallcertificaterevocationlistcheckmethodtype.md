# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>tipo de enum firewallCertificateRevocationListCheckMethodType

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Valores possíveis para firewallCertificateRevocationListCheckMethod
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|0|Nenhum valor configurado por Intune, não substituir o valor padrão de dispositivo configurada pelo usuário|
|nenhum|1|Não verificar a lista de revogação de certificado|
|tentativa|2|Tente verificação CRL e permitir que um certificado somente se o certificado for confirmado pela verificação de|
|exigir|3|Exigir uma verificação CRL bem-sucedida antes de permitir que um certificado|



