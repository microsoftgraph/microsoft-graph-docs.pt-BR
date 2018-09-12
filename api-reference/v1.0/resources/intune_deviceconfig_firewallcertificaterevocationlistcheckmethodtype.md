# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>tipo enumerado firewallCertificateRevocationListCheckMethodType

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Valores possíveis para firewallCertificateRevocationListCheckMethod
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|0|Nenhum valor configurado por Intune, não substituir o valor padrão de dispositivo configurado pelo usuário|
|nenhum|1|Não verificar a lista de revogação de certificado|
|tentativa|2|Tente a verificação CRL e permita um certificado somente se o certificado for confirmado pela verificação|
|precisar|3|Exigir uma verificação CRL bem-sucedida antes de permitir um certificado|








